# Vibe Coding Course: Student Quick Start Guide

## Table of Contents

- [Course Overview](#course-overview)
- [Prerequisites Check](#prerequisites-check)
- [Installation Instructions](#installation-instructions)
- [GitHub Classroom Setup](#github-classroom-setup)
- [How to Accept Assignments](#how-to-accept-assignments)
- [Working with Repositories](#working-with-repositories)
- [Submission Process](#submission-process)
- [Getting Help](#getting-help)
- [Common Issues and Solutions](#common-issues-and-solutions)
- [Document History](#document-history)

---

## Course Overview

### What You'll Learn

- How to use Cursor AI effectively for coding
- End-to-end web development (server → browser)
- Modern AI-assisted development workflow
- Git and GitHub best practices
- Full-stack development basics

### Course Structure

- **Module 1:** Intro to Cursor + GitHub (1h, reading only)
- **Module 2:** Vibe Coding Fundamentals (2-3h, Assignment 1)
- **Module 3:** E2E Hello World (2-4h, Assignment 2)
- **Module 4:** Mini Feature (1-2h, Assignment 3)

**Total time:** 6-10 hours

### Expectations

- You'll use AI tools (Cursor) to generate code
- You'll learn to work with AI effectively
- You'll build a working web application
- You'll document your process and learning

---

## Prerequisites Check

### Required Knowledge

Before starting, you should be comfortable with:

- [ ] Basic programming (variables, functions, control flow)
- [ ] Basic JavaScript knowledge (or willingness to learn with AI)
- [ ] Basic HTML and JavaScript
- [ ] Command line basics
- [ ] Git basics (clone, commit, push)

### Required Tools

You'll need to install:

- [ ] Cursor AI
- [ ] Node.js (v18+)
- [ ] Git
- [ ] Code editor (VS Code recommended)
- [ ] GitHub account

---

## Installation Instructions

### 1. Install Cursor AI

1. Go to [cursor.sh](https://cursor.sh)
2. Click **Download**
3. Install for your operating system
4. Open Cursor
5. Sign up for free account (free tier is sufficient)

**Verify installation:**

- Open Cursor
- You should see the editor interface

**Learn more:**
- Watch the official installation guide: [Building with Cursor - Step 1: Installing and Setting Up Cursor](https://cursorai.notion.site/Building-with-Cursor-public-273da74ef0458051bf22e86a1a0a5c7d)

### 1.1 Understanding Cursor's Interface

After installing Cursor, take a moment to familiarize yourself with the interface:

**Key Interface Elements:**
- **Editor pane:** Where you write and edit code
- **Chat panel:** Where you interact with Cursor AI (`Cmd+K` / `Ctrl+K`)
- **Composer:** Multi-file editing mode (`Cmd+I` / `Ctrl+I`)
- **File explorer:** Navigate your project files
- **Terminal:** Run commands and see output

**Basic Keyboard Shortcuts:**
- `Cmd+K` / `Ctrl+K` - Open chat panel
- `Cmd+I` / `Ctrl+I` - Open Composer (multi-file editing)
- `Cmd+L` / `Ctrl+L` - Toggle chat history
- `Cmd+Shift+P` / `Ctrl+Shift+P` - Command palette

**Learn more:**
- Watch the official interface guide: [Building with Cursor - Step 2: Overview of Cursor's Interface](https://cursorai.notion.site/Building-with-Cursor-public-273da74ef0458051bf22e86a1a0a5c7d)

**Pro tip:** Spend 5-10 minutes exploring the interface before starting assignments. Try opening the chat panel and asking Cursor a simple question to test it out.

### 2. Install Node.js (for Node.js students)

1. Go to [nodejs.org](https://nodejs.org)
2. Download **LTS version** (v18 or higher)
3. Run installer
4. Follow installation wizard

**Verify installation:**

```bash
node --version
# Should show v18.x.x or higher

npm --version
# Should show version number
```

### 3. Verify Node.js Installation

Make sure Node.js is working correctly:

```bash
# Check Node.js version
node --version
# Should show v18.x.x or higher

# Check npm (comes with Node.js)
npm --version
# Should show version number
```

### 4. Install Git

1. Go to [git-scm.com](https://git-scm.com)
2. Download for your operating system
3. Run installer
4. Use default settings

**Verify installation:**

```bash
git --version
# Should show version number
```

### 5. Install VS Code (Recommended)

1. Go to [code.visualstudio.com](https://code.visualstudio.com)
2. Download for your operating system
3. Run installer
4. Install recommended extensions:
   - JavaScript/TypeScript
   - ESLint (optional, for code quality)

### 6. Create GitHub Account

1. Go to [github.com](https://github.com)
2. Click **Sign up**
3. Create account
4. Verify email address
5. Complete profile setup

---

## GitHub Classroom Setup

### 1. Join Course Using Invitation Link

1. **Click the invitation link:**

   - [👉 Join Vibe Coding Course →](https://classroom.github.com/a/zHOCUqGM)
   - Or use the link provided by your teacher

2. **Sign in to GitHub:**

   - If not logged in, GitHub will ask you to sign in
   - Use your GitHub account (or create one at [github.com](https://github.com))

3. **⚠️ If you see a name list (roster):**

   - **Click "Skip to the next step" link** (usually at the bottom of the page)
   - This skips the name list and lets you join directly
   - **You don't need to select your name** - you can always skip this step!

4. **Accept the assignment:**
   - You'll see the course: **"Vibe Coding 2026"**
   - Click **"Accept this assignment"** or **"Accept"**
   - You'll automatically join the classroom too!

### 2. Verify Access

- [ ] You can see the classroom: **"Vibe Coding 2026"**
- [ ] You can see assignments in the **Assignments** tab
- [ ] Your GitHub username is correct
- [ ] You can see your own repositories

---

## How to Accept Assignments

### Step 1: View Assignment

1. In GitHub Classroom, go to **Assignments** tab
2. Find the assignment you want to start
3. Click on the assignment

### Step 2: Accept Assignment

1. Click **Accept this assignment** button
2. GitHub will create a repository for you
3. Wait for repository creation (usually instant)
4. Click **Your assignment repository** link

### Step 3: Clone Repository

1. In your repository, click **Code** button
2. Copy the repository URL
3. Open terminal/command prompt
4. Navigate to where you want to clone:
   ```bash
   cd ~/projects  # or wherever you keep projects
   ```
5. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
6. Navigate into the repository:
   ```bash
   cd <repository-name>
   ```

### Step 4: Verify Setup

- [ ] Repository cloned successfully
- [ ] You can see files in the repository
- [ ] You're ready to start coding!

---

## Working with Repositories

### Opening in Cursor

1. Open Cursor
2. Click **File** → **Open Folder**
3. Select your cloned repository folder
4. You're ready to code!

### Using Cursor AI

1. **Start a chat:**

   - Press `Cmd+K` (Mac) or `Ctrl+K` (Windows/Linux)
   - Type your request

2. **Example prompts:**

   - "Create a Node.js Express server with an endpoint /api/hello that returns { message: 'Hello Vibe!' }"
   - "Create an HTML page that fetches from /api/hello and displays the message"

3. **Review generated code:**
   - Read through the code
   - Understand what it does
   - Modify if needed

### Making Changes

1. **Edit files** in Cursor
2. **Save files** (Cmd+S / Ctrl+S)
3. **Test your code:**
   - Run server: `npm start` or `node server/index.js`
   - Open HTML in browser
   - Verify it works

### Committing Changes

1. **Stage changes:**

   ```bash
   git add .
   ```

2. **Commit changes:**

   ```bash
   git commit -m "Add server endpoint and HTML client"
   ```

3. **Push to GitHub:**
   ```bash
   git push
   ```

### Best Practices

- **Commit often:** Small, frequent commits are better
- **Write clear commit messages:** Describe what you changed
- **Test before committing:** Make sure code works
- **Document your process:** Update README.md

---

## Submission Process

### Before Submitting

- [ ] Code works as required
- [ ] All requirements met
- [ ] README.md updated with:
  - Setup instructions
  - How to run
  - Screenshot of working app
  - Prompts you used (if applicable)
- [ ] All changes committed and pushed

### Submitting Assignment

1. **Push final changes:**

   ```bash
   git add .
   git commit -m "Final submission"
   git push
   ```

2. **Verify on GitHub:**

   - Go to your repository on GitHub
   - Verify all files are there
   - Check README.md is updated

3. **Mark as complete (if required):**
   - Some assignments may have a "Mark as complete" button
   - Click it if available

### After Submission

- RepodIn will automatically analyze your submission
- You'll receive AI feedback in RepodIn Student Dashboard
- Teacher will review and provide feedback
- Check for feedback in both GitHub Classroom and RepodIn

---

## Getting Help

### Help Channel

**Where to ask questions:**

- Discord/Slack/Teams channel (provided by teacher)
- GitHub Classroom discussions
- Office hours (if available)

**What to include:**

- Clear description of the problem
- What you've tried
- Error messages (if any)
- Screenshots (if helpful)

### Resources

**Course Materials:**

- [Building with Cursor (public)](https://cursorai.notion.site/Building-with-Cursor-public-273da74ef0458051bf22e86a1a0a5c7d)
- [FAQ](./vibe-coding-faq.md)
- [Grading Rubrics](./vibe-coding-grading-rubrics.md)

**External Resources:**

- [Express.js Documentation](https://expressjs.com)
- [Node.js Documentation](https://nodejs.org/docs)
- [MDN Web Docs](https://developer.mozilla.org)
- [Git Documentation](https://git-scm.com/doc)

### Peer Support

- Ask classmates for help
- Share approaches (not complete solutions)
- Help others debug
- Learn from each other

---

## Common Issues and Solutions

### Issue: Can't clone repository

**Solution:**

- Verify you accepted the assignment
- Check repository URL is correct
- Make sure Git is installed
- Try: `git clone <url>` again

### Issue: Server won't start

**Node.js:**

```bash
# Check Node.js is installed
node --version

# Install dependencies
npm install

# Start server
npm start
```

**Troubleshooting:**

```bash
# If npm start fails, try:
node server/index.js

# If port is in use:
# Kill process on port 3000 (Windows)
netstat -ano | findstr :3000
taskkill /PID <PID> /F

# Kill process on port 3000 (Mac/Linux)
lsof -ti:3000 | xargs kill
```

### Issue: CORS error in browser

**Solution:**

- Server needs CORS headers
- Add CORS middleware to server
- Example (Node.js/Express):
  ```javascript
  app.use((req, res, next) => {
    res.header('Access-Control-Allow-Origin', '*')
    res.header('Access-Control-Allow-Headers', 'Content-Type')
    next()
  })
  ```

### Issue: Fetch API not working

**Solution:**

- Check server is running
- Verify endpoint URL is correct
- Check browser console for errors
- Make sure CORS is configured

### Issue: Can't push to GitHub

**Solution:**

- Verify you're authenticated: `git config --global user.name` and `git config --global user.email`
- Check repository URL: `git remote -v`
- Try: `git push origin main` (or `master`)

### Issue: Cursor AI not working

**Solution:**

- Verify Cursor is installed and running
- Check you're signed in
- Try restarting Cursor
- Check internet connection

---

## Document History

| Version | Date       | Author                 | Changes         |
| ------- | ---------- | ---------------------- | --------------- |
| 1.0     | 2025-12-20 | RepodIn Education Team | Initial version |
| 1.1     | 2026-01-07 | RepodIn Education Team | Added explicit Cursor installation and interface sections |

---

**Next Review Date:** 2026-03-20
