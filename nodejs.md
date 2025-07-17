1. Q: What is Node.js?
   A: Node.js is a runtime environment that allows JavaScript to run on the server side, built on Chrome's V8 engine.

2. Q: What is the difference between Node.js and JavaScript?
   A: JavaScript is a programming language, whereas Node.js is a runtime environment that executes JavaScript outside the browser.

3. Q: Explain the event-driven architecture of Node.js.
   A: Node.js uses an event-driven, non-blocking I/O model where an event loop handles asynchronous operations without waiting for tasks to complete.

4. Q: What is the difference between synchronous and asynchronous programming in Node.js?
   A: Synchronous programming executes tasks sequentially, blocking further execution. Asynchronous programming allows tasks to execute concurrently without waiting.

5. Q: What is the purpose of the event loop in Node.js?
   A: The event loop processes asynchronous operations, making Node.js non-blocking and efficient.

6. Q: What are streams in Node.js?
   A: Streams are data handling methods used to process files efficiently without loading them into memory. They include readable, writable, duplex, and transform streams.

7. Q: What is the difference between process.nextTick() and setImmediate()?
   A: process.nextTick() executes a callback immediately after the current operation, while setImmediate() schedules execution after the current event loop cycle.

8. Q: What is the role of the require() function in Node.js?
   A: require() is used to import modules in Node.js.

9. Q: What are the different types of modules in Node.js?
   A: Core modules, local modules, and third-party modules.

10. Q: What is the difference between CommonJS and ES6 modules in Node.js?
    A: CommonJS uses require() and module.exports, while ES6 modules use import and export.

11. Q: What is middleware in Express.js?
    A: Middleware functions process requests before sending a response.

12. Q: Explain the purpose of the package.json file.
    A: It contains project metadata and dependencies.

13. Q: How does Node.js handle file operations asynchronously?
    A: Using the fs module with callback-based, promise-based, or async/await methods.

14. Q: What is the purpose of the cluster module in Node.js?
    A: The cluster module enables multi-core execution by spawning worker processes.

15. Q: How do you create an HTTP server in Node.js?
    A: Using the http module:
    js
    const http = require('http');
    const server = http.createServer((req, res) => {
        res.writeHead(200, { 'Content-Type': 'text/plain' });
        res.end('Hello, Node.js!');
    });
    server.listen(3000, () => console.log('Server running on port 3000'));
    

16. Q: What is the difference between fork() and spawn() in Node.js?
    A: fork() creates a new Node.js process, while spawn() runs a new child process.

17. Q: What is the difference between process.env and dotenv?
    A: process.env accesses environment variables, while dotenv loads them from a .env file.

18. Q: How do you handle uncaught exceptions in Node.js?
    A: Using process.on('uncaughtException', callback).

19. Q: What is a promise in Node.js?
    A: A promise is an object representing the eventual completion or failure of an asynchronous operation.

20. Q: Explain the purpose of async/await in Node.js.
    A: async/await simplifies asynchronous code by allowing it to look synchronous.

21. Q: What is an event emitter in Node.js?
    A: EventEmitter allows handling custom events in Node.js.

22. Q: What is CORS in Node.js?
    A: Cross-Origin Resource Sharing (CORS) controls requests between different domains.

23. Q: What is JWT, and how is it used in Node.js?
    A: JSON Web Token (JWT) is used for authentication by encoding user data.

24. Q: What is the purpose of the buffer module?
    A: It provides a way to handle binary data directly in Node.js.

25. Q: What is the difference between readFile and createReadStream?
    A: readFile loads the entire file into memory, while createReadStream reads data in chunks.

26. Q: How do you implement WebSockets in Node.js?
    A: Using the ws module.

27. Q: What is the difference between PUT and PATCH in REST APIs?
    A: PUT replaces a resource, while PATCH updates part of it.

28. Q: What is the purpose of Nodemon in Node.js?
    A: Nodemon automatically restarts the server when file changes occur.

29. Q: What is the role of bcrypt in Node.js?
    A: bcrypt hashes passwords for security.

30. Q: What are worker threads in Node.js?
    A: Worker threads run JavaScript code in parallel threads.

31. Q: What is the difference between session-based and token-based authentication?
    A: Session-based authentication stores user data in memory, while token-based uses JWTs.

32. Q: What is Express.js?
    A: Express.js is a web framework for building Node.js applications.

33. Q: How do you implement error handling in Express.js?
    A: Using middleware functions.

34. Q: What is PM2 in Node.js?
    A: PM2 is a process manager for running Node.js applications in production.

35. Q: How do you handle file uploads in Node.js?
    A: Using the multer module.

36. Q: How do you secure a Node.js application?
    A: Using helmet, CORS policies, rate limiting, and authentication.

37. Q: What is the difference between global and local installation of Node.js modules?
    A: Global modules are available system-wide, while local modules are project-specific.

38. Q: What is the purpose of the crypto module in Node.js?
    A: It provides cryptographic functionalities like hashing and encryption.

39. Q: How do you connect Node.js to a database?
    A: Using modules like mongoose for MongoDB or sequelize for SQL databases.

40. Q: How do you handle concurrency in Node.js?
    A: Using async/await, promises, and worker threads.

41. Q: What is the purpose of the http module in Node.js?
    A: It enables creating HTTP servers and clients.

42. Q: What is the difference between process.exit() and process.kill()?
    A: process.exit() terminates the process, while process.kill() sends a signal.

43. Q: What is a microservice architecture in Node.js?
    A: A software design pattern where an application is divided into small, independent services.

44. Q: How do you implement authentication in a Node.js app?
    A: Using Passport.js or JWT authentication.

45. Q: What is an API gateway in Node.js?
    A: A single entry point for handling API requests.

46. Q: How do you prevent SQL injection in Node.js?
    A: Using parameterized queries and ORM libraries.

47. Q: What is the difference between process.stdin and readline module?
    A: process.stdin reads input, while readline provides an interface for user input.

48. Q: How do you create a CLI tool in Node.js?
    A: Using the readline module and commander.js.

49. Q: What is Helmet in Node.js?
    A: Helmet is a security middleware for Express.js.

50. Q: How do you implement rate limiting in Node.js?
    A: Using express-rate-limit or Redis
