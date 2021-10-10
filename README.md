# Backend Workshop with Express
## What is Express?
Express is a backend framework which is a server side technology that connects to the database. Basically, a browser or a frontend framework will make a request to the backend framework to perform some action which might be reflected in the database.
## Why use Express?

 - Light, Fast, Free
 - Convenient way to build NodeJS app
 - Community-driven, a lot of helper libraries
 
## Node Installation
1. Download node from [NodeJS](https://nodejs.org/en/)
2. Choose the recommended version
3. Run the wizard
4. Use node -v on command prompt to ensure that the installation has been done completely

## Creating a Node App
1. Create a folder in your preferred directory
2. Open the folder in VSCode
3. Open terminal
4. Type the following command:
	`npm init -y`
	`npm install express --save`
	`npm install nodemon --save-dev`

## Hello World
Create a new file named index.js
`const express = require('express');`
`const app = express();`
`const port = 3000;`

`app.get('/', (req, res) => {`
`res.send('Hello World!');`
`})`

`app.listen(port, () => {`
``console.log(`Example app listening at http://localhost:${port}`);``
`})`

Go to package.json and add a new script
`"start": "nodemon index.js"`

Type `npm run start` in the terminal to run your app
