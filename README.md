# Nest.js Project with MongoDB
This is a basic Nest.js project that uses MongoDB as its database. It provides an initial structure for developing a web application using the Nest.js framework alongside the NoSQL MongoDB database.

# Installation
You can clone the repository locally:

git clone <repository_URL>
Navigate to the project directory:

cd nest-mongoose-demo
Install the necessary dependencies:

npm install
Create a .env file at the root of the project and define the MONGO_CNX_STR environment variable with your corresponding database connection.

MONGO_CNX_STR=mongodb+srv://<username>:<password>@<cluster>/<database_name>?retryWrites=true&w=majority
Note that the .env file will not be uploaded to the repository due to the configuration in the .gitignore file.

# Usage
Once you have installed the dependencies and configured your .env file, you can run the application using the following command:

npm start
This will start the development server. You can access the application at http://localhost:8080 by default.

# Project Structure
The project follows a standard directory structure of Nest.js:

src: Contains all the source code of the application.
  app.controller.ts: Main controller of the application.
  app.module.ts: Main module of the application.
  app.service.ts: Main service of the application.
  main.ts: Entry point of the application.
  middlewares: Folder containing custom middlewares.
  users: Folder containing the module and files related to the "users" resource.
  test: Directory for test files.

# Tests
The project includes tests to ensure its proper functioning:

Unit tests
npm run test

End-to-end tests
npm run test:e2e

Test coverage
npm run test:cov
