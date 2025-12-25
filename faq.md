# Vibe Coding Course: Frequently Asked Questions

> **"RepodIn Education turns GitHub Classroom courses into a scalable, measurable, and quality-controlled learning environment."**

**Document Version:** 1.0
**Last Updated:** 2025-12-20
**Status:** Production
**Maintainer:** RepodIn Education Team
---

## Table of Contents

- [Setup Questions](#setup-questions)
- [Assignment Questions](#assignment-questions)
- [Technical Questions](#technical-questions)
- [Cursor AI Questions](#cursor-ai-questions)
- [Grading Questions](#grading-questions)
- [Pro-Level Questions](#pro-level-questions)
- [RepodIn Questions](#repodin-questions)
- [Document History](#document-history)

---

## Setup Questions

### Q: Do I need to pay for Cursor AI?

**A:** No, the free tier of Cursor AI is sufficient for this course. You can sign up for free at [cursor.sh](https://cursor.sh).

### Q: Can I use a different AI coding tool instead of Cursor?

**A:** While Cursor is recommended, you can use other AI coding assistants. However, the course materials are specifically designed for Cursor, so you may need to adapt instructions.

### Q: Do I need both Node.js and Python?

**A:** No, you only need one. Choose either Node.js or Python based on your preference. Both work equally well for this course.

### Q: What if I don't have a GitHub account?

**A:** You need a GitHub account to participate. Create one for free at [github.com](https://github.com). It's required for GitHub Classroom.

### Q: Can I use a different code editor?

**A:** Yes, you can use any code editor. However, VS Code is recommended and works well with Cursor AI.

---

## Assignment Questions

### Q: What if I miss a deadline?

**A:** Check with your teacher about late submission policy. Some assignments may allow late submissions with a penalty, while others may not.

### Q: Can I work on assignments with other students?

**A:** This depends on your teacher's policy. Generally, collaboration on approaches is encouraged, but each student should submit their own work.

### Q: What if I can't complete an assignment?

**A:** Contact your teacher as soon as possible. They can provide guidance or extensions if needed. It's better to communicate early.

### Q: Can I resubmit after the deadline?

**A:** This depends on your teacher's policy. Some assignments may allow resubmission, while others may not. Check with your teacher.

### Q: What if my code doesn't work?

**A:**
- Document what you tried in README.md
- Show your debugging process
- Partial credit may be given for effort and understanding
- Ask for help in the help channel

---

## Technical Questions

### Q: My server won't start. What should I do?

**A:**
1. Check Node.js/Python is installed: `node --version` or `python --version`
2. Install dependencies: `npm install` or `pip install -r requirements.txt`
3. Check for error messages in terminal
4. Verify port is not already in use
5. Ask for help with specific error message

### Q: I'm getting a CORS error. How do I fix it?

**A:** Add CORS headers to your server. For Node.js/Express:
```javascript
app.use((req, res, next) => {
  res.header('Access-Control-Allow-Origin', '*');
  res.header('Access-Control-Allow-Headers', 'Content-Type');
  next();
});
```

### Q: My fetch() isn't working. What's wrong?

**A:**
1. Check server is running
2. Verify endpoint URL is correct (including port number)
3. Check browser console for errors
4. Make sure CORS is configured on server
5. Verify endpoint returns correct JSON format

### Q: How do I test my server locally?

**A:**
1. Start server: `npm start` or `python server/app.py`
2. Open browser to `http://localhost:3000/api/hello`
3. You should see JSON response
4. Open HTML file in browser (or serve via server)
5. Check browser console for errors

### Q: Can I use a different port?

**A:** Yes, but make sure to update your HTML client to use the correct port. Default is usually 3000.

---

## Cursor AI Questions

### Q: How do I write a good prompt for Cursor?

**A:**
- Be specific about what you want
- Include context (what you're building)
- Mention technologies you're using
- Ask for complete solutions, not just snippets
- Example: "Create a Node.js Express server with an endpoint /api/hello that returns { message: 'Hello Vibe!' }"

### Q: What if Cursor generates code that doesn't work?

**A:**
- This is normal! Debugging is part of learning
- Read the error messages
- Ask Cursor to fix the error
- Document your debugging process in README
- This shows understanding and problem-solving

### Q: Should I document all my prompts?

**A:** Yes, especially for Assignment 2. Documenting prompts shows your learning process and helps teachers understand your approach.

### Q: Can I use Cursor for all assignments?

**A:** Yes! Using Cursor is encouraged for all assignments. The course teaches you to use AI tools effectively.

### Q: What if I don't understand the generated code?

**A:**
- Ask Cursor to explain the code
- Read through it line by line
- Look up unfamiliar concepts
- Document what you learned
- Understanding is more important than generating perfect code

---

## Grading Questions

### Q: How are assignments graded?

**A:** See [Grading Rubrics](./grading-rubrics.md) for detailed criteria. Generally:
- Functionality (does it work?)
- Code quality (is it clean and readable?)
- Documentation (is README complete?)
- Process (did you document your approach?)

### Q: Will I lose points for using AI-generated code?

**A:** No! AI-generated code is expected and encouraged. You're assessed on understanding, not originality.

### Q: What if my code has bugs?

**A:** Minor bugs are acceptable if you show understanding. Document what you tried to fix. Partial credit may be given.

### Q: How important is the README?

**A:** Very important! README is worth 20 points in Assignment 2. Include:
- Setup instructions
- How to run
- Screenshot
- Prompts used

### Q: Can I get feedback before submitting?

**A:** Check with your teacher. Some may offer office hours or help channel support.

---

## Pro-Level Questions

### Q: What are pro-level assignments?

**A:** Optional bonus assignments for students who want to go further. See [Pro-Level Assignments](../assignments/assignment-pro.md).

### Q: How many points are pro assignments worth?

**A:** Up to 50 bonus points total (10 points each). They're optional but can boost your grade.

### Q: Do I need to do all pro assignments?

**A:** No, they're optional. Do as many as you want. Each completed assignment adds bonus points.

### Q: When should I start pro assignments?

**A:** After completing Assignment 3. They're extensions of your main project.

### Q: Can I get help with pro assignments?

**A:** Yes, use the help channel. Pro assignments are more challenging, so help is available.

---

## RepodIn Questions

### Q: What is RepodIn?

**A:** RepodIn is an AI-powered platform that analyzes your code submissions and provides feedback. It's integrated with GitHub Classroom.

### Q: Do I need to sign up for RepodIn?

**A:** Your teacher will set this up. You may need to connect your GitHub account. Check with your teacher for specific instructions.

### Q: How do I view feedback in RepodIn?

**A:**
1. Go to RepodIn Student Dashboard
2. Find your course
3. View submissions and feedback
4. See AI analysis results

### Q: When will I get feedback?

**A:** RepodIn analyzes submissions automatically. You should receive feedback within a few minutes of submitting.

### Q: What if I don't see my submission in RepodIn?

**A:**
- Verify you pushed to GitHub
- Check with teacher that course is synced
- Wait a few minutes for sync
- Contact teacher if still not visible

---

## Document History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | 2025-12-20 | RepodIn Education Team | Initial version |

---

**Next Review Date:** 2026-03-20














