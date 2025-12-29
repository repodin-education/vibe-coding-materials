# Vibe Coding Course: Duration & Considerations

## Table of Contents

- [Course Duration](#course-duration)
- [Student Prerequisites](#student-prerequisites)
- [Technology Stack](#technology-stack)
- [Key Considerations](#key-considerations)
- [Installation Requirements](#installation-requirements)
- [Support and Resources](#support-and-resources)
- [Document History](#document-history)

---

## Course Duration

### Total Time Commitment

**6–10 hours of student work** (1–2 weeks part-time)

### Breakdown by Module

| Module | Workload | Notes |
|--------|----------|-------|
| Module 1 – Intro | 1h | Reading only, no submission |
| Module 2 – Fundamentals | 2–3h | Reflection assignment |
| Module 3 – E2E App | 2–4h | Main practical task |
| Module 4 – Mini Feature | 1–2h | Creative extension |

### Suggested Schedules

**Option 1: One Week Intensive**
- Day 1: Module 1 (1h reading)
- Day 2-3: Module 2 (2-3h, Assignment 1)
- Day 4-5: Module 3 (2-4h, Assignment 2)
- Day 6-7: Module 4 (1-2h, Assignment 3)

**Option 2: Two Weeks Part-Time**
- Week 1:
  - Day 1: Module 1 (1h reading)
  - Day 2-3: Module 2 (2-3h, Assignment 1)
  - Day 4-5: Module 3 (2-4h, Assignment 2)
- Week 2:
  - Day 1-2: Module 4 (1-2h, Assignment 3)

**Option 3: Extended (3 Weeks)**
- Week 1: Modules 1-2
- Week 2: Module 3
- Week 3: Module 4 + Pro-level extensions

---

## Student Prerequisites

### Required Knowledge

- **Intermediate programming knowledge**
  - Comfortable with at least one programming language
  - Understanding of basic programming concepts (variables, functions, control flow)
  - Basic understanding of web development (HTML, JavaScript)

### Required Skills

- **Git and GitHub:**
  - Basic Git commands (clone, add, commit, push)
  - GitHub account creation and usage
  - Understanding of repositories and branches

- **Command Line:**
  - Basic terminal/command prompt usage
  - Navigating directories
  - Running commands

- **Web Development Basics:**
  - HTML structure
  - JavaScript basics (variables, functions, DOM manipulation)
  - HTTP requests (fetch API)

- **Either Node.js or Python:**
  - Node.js: Understanding of npm, package.json, basic Express
  - Python: Understanding of pip, requirements.txt, basic Flask

### Recommended Experience

- Previous experience with:
  - Building small web applications
  - Using development tools (VS Code, terminal)
  - Working with APIs or web services
  - Version control (Git)

---

## Technology Stack

### Student Choice: Node.js or Python

Students can choose their preferred stack:

**Option 1: Node.js + Express**
- Runtime: Node.js (v18+)
- Framework: Express.js
- Package manager: npm
- File structure: `server/`, `client/`

**Option 2: Python + Flask**
- Runtime: Python (v3.11+)
- Framework: Flask
- Package manager: pip
- File structure: `server/`, `client/`

### Required Tools

**All Students:**
- Cursor AI (free tier sufficient)
- Git (latest version)
- GitHub account
- Code editor (VS Code recommended)

**Node.js Students:**
- Node.js v18 or higher
- npm (comes with Node.js)

**Python Students:**
- Python 3.11 or higher
- pip (comes with Python)

### Browser Requirements

- Modern browser (Chrome, Firefox, Safari, Edge)
- JavaScript enabled
- Developer tools access (for debugging)

---

## Key Considerations

### AI Tool Access

**Cursor AI:**
- Students need access to Cursor AI
- Free tier is sufficient for this course
- Students should document prompts used in README.md
- Focus on learning effective prompting, not just using AI

**AI Usage Policy:**
- AI-generated code is expected and encouraged
- Assessment focuses on understanding and modification
- Students must document their prompts and workflow

### Code Review vs. AI-Generated Code

**Important Philosophy:**
This course teaches students to use AI tools effectively. Assessment focuses on:

✅ **Assessed:**
- Understanding of generated code
- Ability to debug and modify code
- Quality of prompts used
- Process documentation
- Problem-solving with AI assistance

❌ **Not Assessed:**
- Whether code was AI-generated (expected)
- Manual coding skills (not the focus)
- Code originality (focus on learning process)

**Assessment Strategy:**
- Review README.md for prompt documentation
- Check code comments and understanding
- Evaluate debugging process
- Assess feature implementation quality

### Testing Requirements

**Assignment 2 (E2E Hello World):**
- Basic functionality testing:
  - Server runs without errors
  - Endpoint `/api/hello` returns correct JSON
  - HTML page loads and displays message
  - Fetch API works correctly

**Assignment 3 (Mini Feature):**
- Feature works as described
- No breaking changes to existing functionality
- Code is clean and readable

**Autograding:**
- Optional autograding available for Assignment 2
- See [Autograding Guide](./vibe-coding-autograding.md)

### Plagiarism Detection

**Prevention Strategies:**
- Students work in private repositories
- Each student has unique repository
- RepodIn AI analysis detects code patterns
- Focus on learning process, not code originality

**Assessment Approach:**
- Evaluate understanding through README documentation
- Check for personalized modifications
- Review prompt quality and iteration process
- Assess problem-solving approach

### Learning Outcomes Assessment

**Students should demonstrate:**

1. **AI-Assisted Coding Workflow:**
   - Effective use of Cursor AI
   - Quality prompting techniques
   - Iterative improvement process

2. **Full-Stack Development:**
   - Server setup and configuration
   - API endpoint creation
   - Client-server communication
   - Basic frontend development

3. **Git Workflow:**
   - Repository management
   - Commit practices
   - Push and submission process

4. **Problem-Solving:**
   - Debugging skills
   - Code modification
   - Feature extension
   - Documentation

5. **Professional Practices:**
   - Code organization
   - README documentation
   - Process documentation
   - Self-reflection

---

## Installation Requirements

### For Students

**Required Software:**
1. **Cursor AI**
   - Download from [cursor.sh](https://cursor.sh)
   - Free tier sufficient
   - Installation guide in [Student Guide](./vibe-coding-student-guide.md)

2. **Node.js (for Node.js students)**
   - Download from [nodejs.org](https://nodejs.org)
   - Version 18 or higher
   - Verify: `node --version`

3. **Python (for Python students)**
   - Download from [python.org](https://python.org)
   - Version 3.11 or higher
   - Verify: `python --version`

4. **Git**
   - Download from [git-scm.com](https://git-scm.com)
   - Verify: `git --version`

5. **Code Editor**
   - VS Code recommended
   - Download from [code.visualstudio.com](https://code.visualstudio.com)

**GitHub Account:**
- Create account at [github.com](https://github.com)
- Verify email address
- Connect to GitHub Classroom

### For Teachers

**Required Setup:**
- GitHub Classroom access
- RepodIn Teacher account
- Starter repositories prepared
- Student roster ready

See [GitHub Classroom Setup Guide](./github-classroom-vibe-coding-setup.md) for details.

---

## Support and Resources

### Help Channel

**Recommended Platforms:**
- Discord (recommended for real-time chat)
- Slack (if institution uses it)
- Microsoft Teams (if institution uses it)
- GitHub Discussions (for async Q&A)

**Channel Structure:**
- `#general` - Course announcements
- `#help` - Technical questions
- `#assignments` - Assignment-specific questions
- `#showcase` - Student work sharing (optional)

### Office Hours

**Optional but Recommended:**
- Weekly office hours (1-2 hours)
- Drop-in or scheduled
- Virtual or in-person
- Record sessions for later viewing

### Resources

**Course Materials:**
- [Building with Cursor (public)](https://cursorai.notion.site/Building-with-Cursor-public-273da74ef0458051bf22e86a1a0a5c7d)
- [Student Quick Start Guide](./vibe-coding-student-guide.md)
- [FAQ](./vibe-coding-faq.md)
- [Grading Rubrics](./vibe-coding-grading-rubrics.md)

**External Resources:**
- [Express.js Documentation](https://expressjs.com)
- [Flask Documentation](https://flask.palletsprojects.com)
- [MDN Web Docs](https://developer.mozilla.org)
- [Git Documentation](https://git-scm.com/doc)

### Peer Support

**Encourage:**
- Student collaboration (within guidelines)
- Code review between students
- Sharing solutions and approaches
- Learning from each other

**Guidelines:**
- Share approaches, not complete solutions
- Help debug, don't write code for others
- Document what you learned from peers

---

## Document History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | 2025-12-20 | RepodIn Education Team | Initial version |

---

**Next Review Date:** 2026-03-20















