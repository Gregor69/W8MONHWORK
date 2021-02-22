# Homework: Full Stack Games Hub App

### Learning Objectives

- Understand the relationship between client, server and database
- Be able to navigate a codebase that you haven't written

## Brief

Your boss has asked to you look over the codebase of a full-stack JavaScript application. The front-end is written in JavaScript using React, the back-end uses an Express server and a MongoDB database. Your task is to make yourself familiar with the codebase.

The application includes a README.md with instructions on running the application.

![Overview of the tech stack and tooling with commands](images/tech_stack_with_commands.png)

*Overview of the tech stack and tooling with commands*

*EDIT: Frontend is now written in React with the command to run `npm start`*

## MVP

### Task

Draw a diagram showing the dataflow through the application starting with a form submission, ending with the re-rendering of the page. This will involve a multi-direction data-flow with the client posting data to the server and the server sending data back to the client with the response. Detail the client, server and database in the diagram and include the names of the files involved in the process.

### Questions

1. What is responsible for defining the routes of the `games` resource?
The 'games router' in the server.js file
2. What do you notice about the folder structure?  Whats the client responsible for? Whats the server responsible for?
The client folder and the folder and files within it is responsible for the app's front end, which the server folder and its corresponding folders and files are responsible for the back end.
3. What are the the responsibilities of server.js?
Passing requests to the databases and accessing games date within it. Handling routing requests for 'games router'. Listening for requests made on the specified port.
4. What are the responsibilities of the `gamesRouter`? 
Channelling request to and from the database.
5. What process does the the client (front-end) use to communicate with the server?
It sends 'fetch' requests via the games services file.
6. What optional second argument does the `fetch` method take? And what is it used for in this application? Hint: See [Using Fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch) on the MDN docs
The init method?
7. Which of the games API routes does the front-end application consume (i.e. make requests to)?
Post and delete.
8. What are we using the [MongoDB Driver](http://mongodb.github.io/node-mongodb-native/) for?
To access and use the database.
## Extension

Why do we need to use [`ObjectId`](https://mongodb.github.io/node-mongodb-native/api-bson-generated/objectid.html) from the MongoDB driver?

Add to your diagram the dataflow for removing a game.
