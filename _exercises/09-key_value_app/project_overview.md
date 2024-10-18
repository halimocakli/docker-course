# Building a Key-Value REST API with Docker

Welcome to our hands-on project where we will dive into creating a key-value REST API! 🚀 This project will enhance your skills in Docker and working with multiple containers, as we utilize an Express-based application and a MongoDB database. Let’s roll up our sleeves and get to work!

## Overview

Before we jump into the step-by-step guide, let’s take a moment to see what you should try to implement on your own:

1. **Set up a Docker environment** for both the Express application and the MongoDB database.
2. **Define a user-defined network** to allow communication between the application and the database containers.
3. **Create volumes** for data persistence with the MongoDB container.
4. **Develop API endpoints** for storing, retrieving, updating, and deleting key-value pairs.
5. **Handle errors** with appropriate status codes based on the API logic.
6. **Include a health check endpoint** to verify that your service is up and running.

Now, it's your turn! Give it a shot and try implementing the solution above before checking out the detailed solution recordings.

## Step-by-Step Guide

Follow these steps to build your Key-Value REST API:

1. **Set up your Docker environment**:

   - Create a `Dockerfile` for the Express application.
   - Create a `docker-compose.yml` file to define your services.

2. **Define the network**:

   - In your `docker-compose.yml`, specify a user-defined network for the application and the database to communicate.

3. **Create and configure the MongoDB container**:

   - Use the official MongoDB image.
   - Define a volume for data persistence in the `docker-compose.yml`.

4. **Develop your Express application**:

   - Set up the required packages (e.g., Express, Mongoose).
   - Implement the routes for the following endpoints:
     - `POST /store`: To create a new key-value pair.
     - `GET /store/:key`: To retrieve the value for a specific key.
     - `PUT /store/:key`: To update the value of an existing key.
     - `DELETE /store/:key`: To delete a key-value pair.
     - `GET /health`: To provide a health check.

5. **Handle error responses**:

   - Ensure that your API returns appropriate status codes such as 400, 404, and 204 based on the various conditions outlined.

6. **Run your containers**:

   - Use `docker-compose up` to start your application and the MongoDB database.

7. **Test your API**:
   - Use Postman or a similar tool to test each endpoint and verify that everything is functioning as expected.

## Conclusion

Congratulations on taking steps to build your key-value REST API! This project not only helps you learn about Docker and managing multiple containers but also provides practical experience developing RESTful services. Keep experimenting with your app and continue learning—there's always more to uncover in the world of software development! 🌟

## Lecture Description

In this lecture, we work on building a key-value REST API using Docker, focusing on the implementation of multiple containers, a MongoDB database, and an Express application. Throughout the session, we cover setting up user-defined networks, data persistence with volumes, and crafting various API endpoints to manage key-value pairs effectively.
