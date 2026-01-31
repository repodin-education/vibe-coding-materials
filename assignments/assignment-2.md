# Assignment 2: E2E Hello World (Server → Browser)

## Learning Objectives

By completing this assignment, you will:
- Build a complete end-to-end web application
- Create a server with an API endpoint
- Create a client that consumes the API
- Use Cursor AI to generate code effectively
- Document your development process

---

## Prerequisites

- Completed Assignment 1
- Node.js (v18+) installed
- Cursor AI installed and configured
- Git installed and configured
- Basic understanding of HTTP and APIs

---

## Instructions

### Goal

Build a complete minimal app pipeline:
- A Node.js + Express server
- Returns "Hello World!" from an API endpoint
- Simple static HTML page fetches the message and displays it in the browser
- All generated using Cursor AI

### Step 1: Create the Server

1. Use Cursor AI to generate an Express server
2. Create endpoint: `GET /api/hello`
3. Endpoint should return: `{ message: "Hello World!" }`
4. Server should run on port 3000 (or environment variable PORT)

**Example prompt for Cursor:**
```
Create a Node.js Express server with an endpoint GET /api/hello that returns { message: "Hello World!" }. The server should run on port 3000 and include CORS headers for local development.
```

### Step 2: Create the Client

1. Use Cursor AI to generate an HTML page
2. HTML should:
   - Load with a clean page
   - Call `/api/hello` using `fetch()`
   - Display the message inside `<div id="output"></div>`

**Example prompt for Cursor:**
```
Create an HTML page that fetches from http://localhost:3000/api/hello and displays the message in a div with id="output". Include error handling.
```

### Step 3: Test Your Application

1. **Start the server:**
   - `npm start` or `node server/index.js`

2. **Open the HTML page:**
   - Open `client/index.html` in your browser
   - Or serve it through your server

3. **Verify it works:**
   - You should see "Hello World!" displayed
   - Check browser console for errors
   - Test the endpoint directly: `curl http://localhost:3000/api/hello`

### Step 4: Document Your Process

Update `README.md` with:
- What prompts you used with Cursor AI
- How to run the project (Node.js setup and start commands)
- Screenshot of the working application in browser

### Step 5: Commit and Push

1. Commit all your changes:
   ```bash
   git add .
   git commit -m "Complete Assignment 2: E2E Hello World"
   git push
   ```

---

## Acceptance Criteria

Your submission will be evaluated based on:

- [ ] Server runs without errors
- [ ] Endpoint `/api/hello` exists and works
- [ ] Endpoint returns correct JSON: `{ message: "Hello World!" }`
- [ ] HTML page loads and displays the message
- [ ] Fetch API works correctly
- [ ] README.md includes:
  - [ ] Prompts used
  - [ ] How to run (Node.js setup)
  - [ ] Screenshot of working app
- [ ] All changes committed and pushed

---

## Submission Requirements

1. **Working application:**
   - Node.js + Express server runs and responds correctly
   - Client displays message correctly

2. **Documentation:**
   - Complete README.md with Node.js setup instructions
   - Screenshot included
   - Prompts documented

3. **Code:**
   - All code files present
   - Code is clean and readable
   - Proper file structure

---

## Grading Rubric

See [Grading Rubrics](../materials/grading-rubrics.md) for detailed criteria.

**Total Points:** 100 points

- Functionality: 40 points
- Code Quality: 25 points
- Documentation: 20 points
- Process: 15 points

---

## Tips for Success

- **Use Cursor AI effectively:** Write clear, specific prompts
- **Test incrementally:** Test server first, then client
- **Handle errors:** Add error handling to your fetch call
- **Document everything:** README is worth 20 points
- **Take screenshot:** Include screenshot of working app

---

## Common Issues and Solutions

### Server won't start
- Check Node.js is installed: `node --version`
- Install dependencies: `npm install`
- Check port is not already in use

### CORS error
- Add CORS headers to server
- See [Student Guide](../materials/student-guide.md) for examples

### Fetch not working
- Check server is running
- Verify endpoint URL is correct
- Check browser console for errors

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
| 1.1 | 2025-12-28 | RepodIn Education Team | Simplified to Node.js only, removed Python option |

---

**Next Review Date:** 2026-03-20














