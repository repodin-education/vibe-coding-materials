# Vibe Coding – Building with Cursor: Complete Course Package

> **"RepodIn Education turns GitHub Classroom courses into a scalable, measurable, and quality-controlled learning environment."**

**Document Version:** 1.0
**Last Updated:** 2025-12-20
**Status:** Production
**Maintainer:** RepodIn Education Team
---

## Table of Contents

- [Course Overview](#course-overview)
- [Course Structure](#course-structure)
- [Assignments](#assignments)
- [Submission Guidelines](#submission-guidelines)
- [Timeline and Duration](#timeline-and-duration)
- [Teacher Preparation](#teacher-preparation)
- [Important Considerations](#important-considerations)
- [RepodIn Integration](#repodin-integration)
- [Document History](#document-history)

---

## Course Overview

### Course Title
**Vibe Coding – Building with Cursor**

### Level
Beginner → Pro foundations

### Duration
1–2 weeks part-time (6–10 hours total)

### Platform
GitHub Classroom

### Focus
End-to-end coding workflow using Cursor, Git, GitHub Repos, and GitHub Classroom submissions.

### Course Goal
Students learn how to build small, high-vibe software features using Cursor + GitHub. The course is based on the excellent material: *"Building with Cursor"* (public). Students will:

- Set up a development environment with Cursor
- Learn the workflow: generate → review → run → debug → push
- Build a small end-to-end "Hello from Server to Browser" app
- Submit assignments using GitHub Classroom
- Practice modern AI-assisted coding patterns

---

## Course Structure

### Module 1 — Intro to Cursor + GitHub

**Duration:** 1 hour (reading only)

**Content:**
- What is Cursor?
- How AI coding workflow differs from manual coding
- Git workflow recap (commit → push → PR)

**Deliverable:** No submission, reading only.

**Resources:**
- [Building with Cursor (public)](https://cursorai.notion.site/Building-with-Cursor-public-273da74ef0458051bf22e86a1a0a5c7d)

---

### Module 2 — Vibe Coding Fundamentals

**Duration:** 2–3 hours

**Content:**
Based on Cursor's "Building with Cursor" guide. Students learn:
- Good prompting techniques
- How to write clear tasks for the AI
- Multi-file reasoning
- Iteration loops
- Debug-first workflow
- Safe refactors

**Assignment 1:** *Cursor Fundamentals Reflection*

Students answer 4 concept questions in `answers.md`:
1. What is Cursor's multi-file reasoning and why is it useful?
2. How would you phrase a "good task prompt" in Cursor? Give 1–2 examples.
3. What is your workflow when debugging an error with Cursor?
4. What is the biggest benefit of AI-assisted coding for you personally?

**Submission:** Push to GitHub repo.

---

### Module 3 — End-to-End "Hello World" (Server → Browser)

**Duration:** 2–4 hours

**Goal:** Build a full minimal app pipeline:
- A Node.js or Python server (student chooses)
- Returns "Hello Vibe!" from an API endpoint
- Simple static HTML page fetches the message and displays it in the browser
- All generated using Cursor

**Assignment 2:** *E2E Hello World Build*

**Requirements:**
1. **Server** (choose one):
   - Node.js + Express **or**
   - Python + Flask
   
   Endpoint: `GET /api/hello` → returns: `{ message: "Hello Vibe!" }`

2. **Browser:**
   - `index.html` that:
     - Loads with a clean page
     - Calls `/api/hello` using `fetch()`
     - Displays the message inside `<div id="output"></div>`

3. **Workflow:**
   - Use Cursor to generate files
   - Run locally
   - Commit → push
   - Add a short explanation in `README.md`:
     - Which language they chose
     - What prompts they used
     - Screenshot of browser output

**Submission:** The working app in GitHub repo.

---

### Module 4 — Final Mini-Feature

**Duration:** 1–2 hours

Students extend the basic app by adding one small "vibe feature", for example:
- Add a timestamp: "Hello Vibe! The time is 12:30."
- Add a button "Refresh Message"
- Add a `/api/vibe` endpoint returning random vibes
- Add CSS styling
- Add server console logging
- Add error-handling message

**Assignment 3:** *Mini Feature Implementation*

**Requirements:**
- Extend Hello World app with **one new feature**
- Update the repo + describe the feature in `README.md`

**Submission:** Extended app with documentation.

---

## Assignments

### Assignment 1: Cursor Fundamentals Reflection

**Goal:** Ensure students understand the principles of building with Cursor.

**Instructions:**
Read the Cursor guide: *Building with Cursor (public)*. Then answer the following in `answers.md`:

1. What is Cursor's multi-file reasoning and why is it useful?
2. How would you phrase a "good task prompt" in Cursor? Give 1–2 examples.
3. What is your workflow when debugging an error with Cursor?
4. What is the biggest benefit of AI-assisted coding for you personally?

**Submission:** Push to GitHub repo.

**Grading:** See [Grading Rubrics](../education/vibe-coding-grading-rubrics.md)

---

### Assignment 2: E2E Hello World (Server → Browser)

**Goal:** Build a complete minimal app pipeline.

**Requirements:**

#### 1. Server
Create server in either:
- Node + Express **or**
- Python + Flask

Endpoint: `GET /api/hello` → returns: `{ message: "Hello Vibe!" }`

#### 2. Browser
`index.html` that:
- Loads with a clean page
- Calls `/api/hello` using `fetch()`
- Displays the message inside `<div id="output"></div>`

#### 3. Workflow
Student must:
- Use Cursor to generate files
- Run locally
- Commit → push
- Add a short explanation in `README.md`:
  - Which language they chose
  - What prompts they used
  - Screenshot of browser output

**Submission:** The working app in GitHub repo.

**Grading:** See [Grading Rubrics](../education/vibe-coding-grading-rubrics.md)

---

### Assignment 3: Mini Feature Implementation

**Goal:** Extend the Hello World app with one new feature.

**Instructions:**
Student extends their Hello World app with **one new feature**. Examples (they choose one):
- Add a timestamp: "Hello Vibe! The time is 12:30."
- Add a button "Refresh Message"
- Add a `/api/vibe` endpoint returning random vibes
- Add CSS styling
- Add server console logging
- Add error-handling message

**Requirements:**
- Feature works as described
- Code is clean and readable
- Feature is documented in `README.md`

**Submission:** Update the repo + describe the feature in `README.md`.

**Grading:** See [Grading Rubrics](../education/vibe-coding-grading-rubrics.md)

---

## Submission Guidelines

### General Requirements

1. **All code must be in GitHub Classroom repository**
2. **All submissions must be pushed before deadline**
3. **README.md must include:**
   - Which language/stack was chosen
   - What prompts were used (for Cursor AI)
   - How to run the project
   - Screenshots of working application

### Assignment-Specific Requirements

**Assignment 1:**
- Create `answers.md` file
- Answer all 4 questions
- Push to repository

**Assignment 2:**
- Working server (Node.js or Python)
- Working HTML client
- Server must run on localhost
- Client must successfully fetch and display message
- README.md with setup instructions

**Assignment 3:**
- Extended app with new feature
- Feature must work as described
- README.md updated with feature description

---

## Timeline and Duration

### Recommended Timeline

**Total length:** 6–10 hours of student work

| Module | Workload | Notes |
|--------|----------|-------|
| Module 1 – Intro | 1h | Reading only |
| Module 2 – Fundamentals | 2–3h | Reflection assignment |
| Module 3 – E2E App | 2–4h | Main practical task |
| Module 4 – Mini Feature | 1–2h | Creative extension |

This fits well for a **one-week sprint** or **two weeks part-time**.

### Suggested Schedule

**Option 1: One Week Intensive**
- Day 1: Module 1 (reading)
- Day 2-3: Module 2 (Assignment 1)
- Day 4-5: Module 3 (Assignment 2)
- Day 6-7: Module 4 (Assignment 3)

**Option 2: Two Weeks Part-Time**
- Week 1:
  - Day 1: Module 1 (reading)
  - Day 2-3: Module 2 (Assignment 1)
  - Day 4-5: Module 3 (Assignment 2)
- Week 2:
  - Day 1-2: Module 4 (Assignment 3)

---

## Teacher Preparation

### Before Course Starts

- [ ] GitHub Classroom setup completed
- [ ] Starter repositories created and marked as templates
- [ ] All assignments created in GitHub Classroom
- [ ] Student roster imported
- [ ] Help channel set up (Discord/Slack/Teams)
- [ ] Installation guide reviewed
- [ ] Grading rubrics prepared
- [ ] First assignment ready to release

### During Course

- [ ] Monitor student progress in RepodIn Dashboard
- [ ] Provide timely feedback on submissions
- [ ] Answer questions in help channel
- [ ] Track late submissions
- [ ] Identify struggling students early

### After Course

- [ ] Review all submissions
- [ ] Export grades to GitHub Classroom
- [ ] Collect student feedback
- [ ] Update course materials based on feedback

For detailed checklists, see:
- [Teacher Checklist](./vibe-coding-teacher-checklist.md)
- [Student Checklist](./vibe-coding-student-checklist.md)

---

## Important Considerations

### Student Prerequisites

- Intermediate programming knowledge
- Basic understanding of:
  - Git and GitHub
  - Command line
  - Web development basics (HTML, JavaScript)
  - Either Node.js or Python

### Technology Requirements

**Students must install:**
- Cursor AI (free tier available)
- Node.js (v18+) **or** Python (v3.11+)
- Git
- GitHub account

### AI Tool Access

- Students need access to Cursor AI
- Free tier is sufficient for this course
- Students should document prompts used

### Code Review vs. AI-Generated Code

**Important:** This course teaches students to use AI tools effectively. Assessment focuses on:
- Understanding of generated code
- Ability to debug and modify code
- Quality of prompts used
- Process documentation

**Not assessed:**
- Whether code was AI-generated (expected)
- Manual coding skills (not the focus)

### Testing Requirements

- Assignment 2: Basic functionality testing (server runs, endpoint works, client displays message)
- Assignment 3: Feature works as described
- Autograding available for Assignment 2 (optional)

### Plagiarism Detection

- Students work in private repositories
- RepodIn AI analysis detects code patterns
- Focus on learning process, not code originality

### Learning Outcomes Assessment

Students should demonstrate:
1. Understanding of AI-assisted coding workflow
2. Ability to prompt AI effectively
3. Basic full-stack development skills
4. Git workflow proficiency
5. Problem-solving with AI tools

### Support and Resources

**Help Channel:**
- Discord/Slack/Teams channel for questions
- Office hours (optional)
- Peer support encouraged

**Resources:**
- [Building with Cursor (public)](https://cursorai.notion.site/Building-with-Cursor-public-273da74ef0458051bf22e86a1a0a5c7d)
- [Student Quick Start Guide](./vibe-coding-student-guide.md)
- [FAQ](./vibe-coding-faq.md)

---

## RepodIn Integration

### Overview

This "Vibe Coding" course is designed to work seamlessly with RepodIn's Teacher Dashboard and Student Dashboard.

### Integration Workflow

```
1. Create Course in GitHub Classroom
   ↓
2. Sync to RepodIn Teacher Dashboard
   ↓
3. Enable AI Analysis in RepodIn
   ↓
4. Students submit via GitHub Classroom
   ↓
5. RepodIn analyzes automatically
   ↓
6. Teacher reviews in RepodIn Dashboard
   ↓
7. Export grades back to GitHub Classroom
```

### Key Benefits

**For Teachers:**
- Single dashboard for all student submissions
- Automatic AI analysis of code quality
- Progress tracking and analytics
- Time-saving: 2-3 minutes per student vs. 15-30 minutes manually

**For Students:**
- Immediate AI feedback on submissions
- Clear visibility into progress
- Actionable improvement suggestions
- Self-assessment before teacher review

### Setup Steps

1. **Create Course in GitHub Classroom**
   - Follow [GitHub Classroom Setup Guide](./github-classroom-vibe-coding-setup.md)

2. **Sync to RepodIn**
   - Connect GitHub account in RepodIn Teacher Dashboard
   - Import course from GitHub Classroom
   - Enable auto-sync for new submissions

3. **Configure AI Analysis**
   - Select analysis template for "Vibe Coding" course
   - Set up automatic analysis on submission
   - Configure grading criteria

4. **Monitor and Grade**
   - View all submissions in RepodIn Dashboard
   - Review AI analysis results
   - Add teacher comments and scores
   - Export grades to GitHub Classroom

For detailed integration instructions, see:
- [RepodIn Integration Guide](./vibe-coding-repodin-integration.md)
- [Student RepodIn Guide](./vibe-coding-student-repodin-guide.md)

---

## Document History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | 2025-12-20 | RepodIn Education Team | Initial version |

---

**Next Review Date:** 2026-03-20














