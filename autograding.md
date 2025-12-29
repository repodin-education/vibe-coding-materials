# Vibe Coding Course: Autograding Configuration Guide

## Table of Contents

- [Overview](#overview)
- [When to Use Autograding](#when-to-use-autograding)
- [Assignment 2: E2E Hello World Autograding](#assignment-2-e2e-hello-world-autograding)
- [Assignment 3: Mini Feature Autograding](#assignment-3-mini-feature-autograding)
- [GitHub Actions Workflow Examples](#github-actions-workflow-examples)
- [Troubleshooting](#troubleshooting)
- [Document History](#document-history)

---

## Overview

### What is Autograding?

Autograding automatically tests student submissions using GitHub Actions. It provides immediate feedback to students and reduces manual grading time.

### Benefits

- **Immediate feedback:** Students know if their code works
- **Time savings:** Reduces manual testing time
- **Consistency:** Same tests for all students
- **Learning:** Students can iterate until tests pass

### Limitations

- **Functionality only:** Tests if code works, not code quality
- **Not comprehensive:** Can't test all aspects
- **Manual review still needed:** For code quality, documentation, process

---

## When to Use Autograding

### Recommended: Assignment 2

**Why:**
- Clear, testable requirements
- Binary pass/fail criteria
- Reduces manual testing burden
- Students get immediate feedback

**What to test:**
- Server runs
- Endpoint exists
- Returns correct JSON
- HTML page loads
- Fetch works

### Optional: Assignment 3

**Why:**
- Feature requirements vary
- Harder to create universal tests
- May need custom tests per feature

**What to test:**
- Feature exists
- Feature works as described
- No breaking changes

### Not Recommended: Assignment 1

**Why:**
- Reflection questions
- No code to test
- Requires human evaluation

---

## Assignment 2: E2E Hello World Autograding

### Test Requirements

**Server Tests:**
1. Server starts without errors
2. Endpoint `/api/hello` exists
3. Endpoint returns correct JSON format
4. Endpoint returns correct message: `"Hello Vibe!"`

**Client Tests:**
1. HTML file exists
2. HTML file contains fetch API call
3. HTML file displays message

### Node.js Autograding Workflow

See [Node.js Starter Repository](../setup/starter-repos/nodejs-starter/.github/workflows/autograding.yml) for complete example.

**Key Tests:**
```yaml
- name: Test endpoint exists
  run: |
    response=$(curl -s http://localhost:3000/api/hello)
    echo "$response" | grep -q "Hello Vibe!" || exit 1

- name: Test JSON format
  run: |
    response=$(curl -s http://localhost:3000/api/hello)
    echo "$response" | jq -e '.message' || exit 1
```

### Python Autograding Workflow

See [Python Starter Repository](../setup/starter-repos/python-starter/.github/workflows/autograding.yml) for complete example.

**Key Tests:**
```yaml
- name: Test endpoint exists
  run: |
    response=$(curl -s http://localhost:3000/api/hello)
    echo "$response" | grep -q "Hello Vibe!" || exit 1

- name: Test JSON format
  run: |
    response=$(curl -s http://localhost:3000/api/hello)
    echo "$response" | python -m json.tool || exit 1
```

### Setup in GitHub Classroom

1. **Enable Autograding:**
   - In assignment settings, check "Enable autograding"
   - Select test file or workflow

2. **Configure Tests:**
   - Use provided workflow files
   - Or create custom tests
   - Set timeout (recommended: 5 minutes)

3. **Test Configuration:**
   - Test with sample submission
   - Verify tests pass/fail correctly
   - Adjust as needed

---

## Assignment 3: Mini Feature Autograding

### Challenges

- **Feature variety:** Students choose different features
- **Hard to test universally:** Each feature needs different tests
- **Optional:** May skip autograding for this assignment

### If Using Autograding

**Basic Tests:**
- Server still runs
- Existing functionality still works
- No breaking changes

**Feature-Specific Tests:**
- Create tests for common features
- Or skip autograding for this assignment
- Focus on manual review

### Recommended Approach

**Option 1: Skip Autograding**
- Manual review only
- Focus on code quality and documentation
- More flexible assessment

**Option 2: Basic Tests Only**
- Test that server still works
- Test that existing functionality preserved
- Don't test new feature (too variable)

---

## GitHub Actions Workflow Examples

### Node.js Complete Workflow

```yaml
name: Autograding - Assignment 2

on:
  push:
    branches: [main, master]
  pull_request:
    branches: [main, master]

jobs:
  autograde:
    runs-on: ubuntu-latest
    timeout-minutes: 5

    steps:
      - name: Checkout code
        uses: actions/checkout@v4

      - name: Setup Node.js
        uses: actions/setup-node@v4
        with:
          node-version: '20'
          cache: 'npm'

      - name: Install dependencies
        run: npm ci

      - name: Start server
        run: npm start &
        env:
          PORT: 3000

      - name: Wait for server
        run: |
          timeout 30 bash -c 'until curl -f http://localhost:3000/api/hello; do sleep 1; done'

      - name: Test endpoint exists
        run: |
          response=$(curl -s http://localhost:3000/api/hello)
          echo "$response" | grep -q "Hello Vibe!" || exit 1

      - name: Test JSON format
        run: |
          response=$(curl -s http://localhost:3000/api/hello)
          echo "$response" | jq -e '.message' || exit 1

      - name: Test HTML file exists
        run: |
          test -f client/index.html || exit 1

      - name: Test HTML has fetch
        run: |
          grep -q "fetch" client/index.html || exit 1
```

### Python Complete Workflow

```yaml
name: Autograding - Assignment 2

on:
  push:
    branches: [main, master]
  pull_request:
    branches: [main, master]

jobs:
  autograde:
    runs-on: ubuntu-latest
    timeout-minutes: 5

    steps:
      - name: Checkout code
        uses: actions/checkout@v4

      - name: Setup Python
        uses: actions/setup-python@v4
        with:
          python-version: '3.11'

      - name: Install dependencies
        run: pip install -r requirements.txt

      - name: Start server
        run: python server/app.py &
        env:
          PORT: 3000

      - name: Wait for server
        run: |
          timeout 30 bash -c 'until curl -f http://localhost:3000/api/hello; do sleep 1; done'

      - name: Test endpoint exists
        run: |
          response=$(curl -s http://localhost:3000/api/hello)
          echo "$response" | grep -q "Hello Vibe!" || exit 1

      - name: Test JSON format
        run: |
          response=$(curl -s http://localhost:3000/api/hello)
          echo "$response" | python -m json.tool || exit 1

      - name: Test HTML file exists
        run: |
          test -f client/index.html || exit 1

      - name: Test HTML has fetch
        run: |
          grep -q "fetch" client/index.html || exit 1
```

---

## Troubleshooting

### Common Issues

**Issue: Tests fail but code works locally**

**Solutions:**
- Check server port (may need to be 3000)
- Verify dependencies are installed
- Check for environment-specific issues
- Review workflow logs for errors

**Issue: Server won't start in workflow**

**Solutions:**
- Check package.json/requirements.txt
- Verify start command is correct
- Check for missing dependencies
- Review error logs

**Issue: Timeout errors**

**Solutions:**
- Increase timeout (default: 5 minutes)
- Check server starts quickly
- Verify wait logic works

**Issue: Tests pass but manual review shows issues**

**Solutions:**
- Autograding tests functionality only
- Manual review still needed for:
  - Code quality
  - Documentation
  - Process understanding

### Getting Help

- Review GitHub Actions logs
- Test workflow locally first
- Check starter repository examples
- Ask in help channel

---

## Document History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | 2025-12-20 | RepodIn Education Team | Initial version |

---

**Next Review Date:** 2026-03-20














