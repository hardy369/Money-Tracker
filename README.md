MERN Stack Full-Stack Application
This is a simple full-stack application built using the MERN stack: MongoDB, Express, React, and Node.js. This project provides a basic setup for connecting the backend API with the frontend, as well as integrating MongoDB for data storage.

Table of Contents
Installation
Backend Setup
Frontend Setup
Running the Application
Database Setup
Troubleshooting
License
Installation
Prerequisites:
Before proceeding, make sure you have the following installed:

Node.js
Yarn (or you can use npm)
1. Clone the repository:
2. Install dependencies:
In the root directory, install the necessary dependencies for both the backend and the frontend:
yarn install
This will install dependencies for both the frontend and backend directories.

4. Install Backend-specific dependencies:
In case you missed some dependencies, navigate to the api folder (backend) and run:
cd api
yarn add express cors
Backend Setup
Configure the API:

The backend is built with Express and uses MongoDB for data storage.
Navigate to the api folder and ensure that you have set up the connection to MongoDB correctly in the index.js file (or your main backend file).
Example of a MongoDB connection string :

bash
Copy
node index.js
This should start the backend API and confirm if it's connected successfully to MongoDB.

Frontend Setup
Configure Frontend:

The frontend is built with React. It should be configured to make API calls to the backend.
Ensure the correct backend API endpoint is being used. You may need to modify the base URL of API requests in your React code to match the backend's URL.
Run the Frontend: From the root of the project, navigate to the src folder and run:

yarn start
This will launch the React development server. Your frontend should now be up and running locally, and it should connect to the backend.

Running the Application
Once both the backend and frontend are set up, you can run both servers:
Navigate to the api folder and start the backend with node index.js.


The frontend will be running on http://localhost:3000.
The backend will be running on http://localhost:4000 (or whichever port you configured in your backend).


Database Setup
MongoDB Configuration:

Ensure you have a MongoDB database set up. 
Database Connection Troubleshooting:
Check connection string: Ensure there are no typos in the connection string and that it's correctly formatted.Double-check your MongoDB URI, username, password, and the host to ensure there are no errors in the string.
Database User Password: Ensure the password in the connection string is not wrapped in angular brackets (<password>).
Troubleshooting
Port Conflicts: Ensure the port you're using for your backend is not in use by another application. If the port is already in use, try using another port not in use.


