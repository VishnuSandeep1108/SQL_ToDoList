# TODO List using Node.js, Express, and MySQL

## Overview

This guide will walk you through setting up a basic TODO list application using Node.js, Express, and MySQL. Follow the steps below to set up the project and build a RESTful API for managing your tasks.

## Getting Started

1. **Initialize your project**: Run `npm init` to create a `package.json` file. Install the required dependencies using the following command:

    ```bash
    npm install express body-parser mysql --save
    ```

2. **Database Setup**: Create a MySQL database with the schema provided in `db/schema.sql`. Populate the table with sample data using `db/seeds.sql`.

3. **Connection Pool**: Implement a connection pool to the database in `app/config/connection.js`.

4. **Model Creation**: Develop a model for interacting with the database in `app/models/todo.js`. Include the connection module and create methods for CRUD operations.

5. **Route Handling**: Set up routes in `app/controllers/routes.js` to define how the model methods will be called. Include the model module and create routes for GET, POST, PUT, and DELETE HTTP requests.

6. **Integration in Main App**: Include the connection and router modules in `app.js`. Call them before `app.listen()` to ensure proper functioning.

## Additional Resources

If you encounter any issues or want to enhance your understanding, check out the following resources:

- [Node.js Documentation](https://nodejs.org/en/docs/)
- [Express.js Documentation](https://expressjs.com/)
- [MySQL Documentation](https://dev.mysql.com/doc/)