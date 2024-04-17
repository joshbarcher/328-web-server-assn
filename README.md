### Assignment: Node.js Basic Web Server

**Course:** Year-3 Back-end Web Development  
**Technology:** Node.js  
**Deadline:** [Insert Deadline Here]  
**Submission Format:** Zip file containing the project directory

#### Introduction
Understanding how web servers work is crucial for any software developer. This assignment will introduce you to the basics of building a web server using Node.js, focusing on serving static files and handling basic routing. You will not use Express.js for this project to reinforce your understanding of Node.js core modules.

#### Objectives
1. Create a Node.js project from scratch.
2. Build a simple web server that can serve static files.
3. Understand and implement basic routing within your server.

#### Project Setup
1. **Create a new Node.js project.** Initialize a Node.js project with a `package.json` file. Make sure to set `"type": "module"` to enable ES Module syntax.
2. **Install necessary npm packages:**
   - `chalk`: For adding colors to your console outputs.
   - `nodemon`: For automatically restarting your server during development. Use this in your `npm run dev` script.
3. **Project Structure:** Organize your project folder as follows:
   - `public/`: Directory for static files.
     - `home.html`: Basic HTML page.
     - `home.css`: CSS for styling your HTML page.
     - `me.png`: An image file representing you.
   - `server.js`: Your main server configuration and startup script.
   - `package.json`: Includes all dependencies and scripts.

#### Building the Web Server
1. **Server Configuration:**
   - Use Node’s `http` module to create a server.
   - Start the server on `localhost:3000`.
   - Implement console logging to show each requested URL path when a request is made. Example: "Request for /home".
2. **Serving Static Files:**
   - Utilize the `fs` module to read files from the `public` directory and serve them in response to HTTP requests.
   - Handle different types of files correctly, sending them with a HTTP 200 status code if found.
   - Return a 404 status if a requested file is not found.

#### HTML and CSS Files
- **home.html**: Should include:
  - Your name.
  - Your picture (`me.png`).
  - A brief biography of your experience as a web developer.
  - A roadmap of your upcoming web development courses and the technologies you will learn.
- **Accessibility:** Ensure that `home.html` can be accessed via:
  - `localhost:3000` (default)
  - `localhost:3000/home` (custom route)
  - `localhost:3000/home.html` (standard URL)

#### Testing
- Place provided test files (HTML, CSS, JS, images, fonts) into the `public` directory. Ensure each file loads correctly on `localhost:3000` with related resources.

#### Submission Instructions
- Zip your project directory, ensuring all necessary files are included.
- Submit the zip file via the course submission portal by the deadline.

#### Helpful Hints
- **Debugging:** Use `nodemon` for active debugging during development; it refreshes your server automatically after changes.
- **File Paths:** Pay close attention to file paths when linking resources in HTML and CSS.
- **Error Handling:** Implement basic error handling when files are not found to avoid server crashes.

Good luck, and have fun learning the inner workings of web servers with Node.js!