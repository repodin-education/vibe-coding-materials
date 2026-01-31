# Assignment 3: Mini Feature Implementation

> **"RepodIn Education is a teacher-first management and analytics layer on top of GitHub Classroom."**

**Document Version:** 1.0
**Last Updated:** 2025-12-20
**Status:** Production
**Maintainer:** RepodIn Education Team
---

## Learning Objectives

By completing this assignment, you will:
- Extend an existing application with new functionality
- Practice feature planning and implementation
- Integrate new code with existing codebase
- Document feature implementation
- Demonstrate creativity and problem-solving

---

## Prerequisites

- Completed Assignment 2 (E2E Hello World)
- Working Node.js server and client from Assignment 2
- Understanding of Node.js + Express basics
- Cursor AI installed and configured

---

## Instructions

### Goal

Extend your Hello World app from Assignment 2 with **one new feature**. Choose a feature that adds value and demonstrates your understanding.

### Step 1: Choose Your Feature

Select one feature from the examples below, or create your own:

#### Example Features:

1. **Timestamp Feature:**
   - Display current time with message: "Hello Vibe! The time is 12:30."
   - Server returns current timestamp
   - Client displays formatted time

2. **Refresh Button:**
   - Add a button "Refresh Message"
   - Clicking button fetches new message
   - Updates display without page reload

3. **Random Vibes Endpoint:**
   - Create new endpoint `/api/vibe`
   - Returns random positive messages
   - Client can fetch random vibes

4. **CSS Styling:**
   - Add attractive CSS styling
   - Make page visually appealing
   - Responsive design (optional)

5. **Server Logging:**
   - Add console logging to server
   - Log requests and responses
   - Track usage

6. **Error Handling:**
   - Add error handling message
   - Display user-friendly errors
   - Handle network failures gracefully

**Or create your own feature!** Be creative, but keep it simple and focused.

### Step 2: Plan Your Feature

1. **Document your plan:**
   - What feature will you add?
   - How will it work?
   - What changes are needed?

2. **Consider integration:**
   - How does it fit with existing code?
   - Will it break existing functionality?
   - What files need to be modified?

### Step 3: Implement Your Feature

1. **Use Cursor AI:**
   - Generate code for your feature
   - Integrate with existing code
   - Test as you go

2. **Example prompts:**
   - "Add a timestamp to the hello message that shows the current time"
   - "Add a refresh button that fetches a new message when clicked"
   - "Create a new endpoint /api/vibe that returns random positive messages"

3. **Test your feature:**
   - Make sure it works
   - Verify no breaking changes
   - Test edge cases

### Step 4: Document Your Feature

Update `README.md` with:
- **Feature description:** What did you add?
- **How to use:** How does the feature work?
- **Screenshots/demos:** Visual proof it works
- **Technical details:** How was it implemented?

### Step 5: Commit and Push

1. Commit all your changes:
   ```bash
   git add .
   git commit -m "Complete Assignment 3: Mini Feature - [your feature name]"
   git push
   ```

---

## Acceptance Criteria

Your submission will be evaluated based on:

- [ ] Feature works as described
- [ ] No breaking changes to existing functionality
- [ ] Code is clean and well-integrated
- [ ] Feature is documented in README.md
- [ ] Screenshots/demos included
- [ ] All changes committed and pushed

---

## Submission Requirements

1. **Working feature:**
   - Feature works as described
   - No breaking changes
   - Well-integrated with existing code

2. **Documentation:**
   - Feature described in README.md
   - How to use documented
   - Screenshots included

3. **Code quality:**
   - Clean, readable code
   - Follows existing patterns
   - Proper error handling

---

## Grading Rubric

See [Grading Rubrics](../materials/grading-rubrics.md) for detailed criteria.

**Total Points:** 100 points

- Feature Implementation: 40 points
- Code Quality: 25 points
- Documentation: 20 points
- Creativity & Complexity: 15 points

---

## Tips for Success

- **Keep it simple:** One focused feature is better than many incomplete ones
- **Test thoroughly:** Make sure nothing breaks
- **Document well:** README is worth 20 points
- **Be creative:** Show your problem-solving skills
- **Use Cursor AI:** Generate code, then understand and modify it

---

## Common Issues and Solutions

### Feature breaks existing code
- Test existing functionality after adding feature
- Revert if needed and try different approach
- Test incrementally

### Feature too complex
- Simplify your approach
- Focus on one thing that works well
- You can always extend later

### Feature too simple
- Add some complexity
- Make it more interesting
- Show your skills

---

## Getting Help

- Ask questions in the help channel
- Review [Student Guide](../materials/student-guide.md)
- Check [FAQ](../materials/faq.md)
- Contact your teacher if needed

---

## Document History

| Version | Date | Author | Changes |
|---------|------|--------|---------|
| 1.0 | 2025-12-20 | RepodIn Education Team | Initial version |

---

**Next Review Date:** 2026-03-20














