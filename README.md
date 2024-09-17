## Introduction
This project serves as a basic template for connecting a MongoDB database to a MERN application using Mongoose as the Object Data Modeling (ODM) library. The project is split into a backend (Node.js + Express.js) that connects to MongoDB and a frontend built with React.

## Technologies Used
- **MongoDB** - NoSQL database
- **Express.js** - Web framework for Node.js
- **React.js** - Frontend framework
- **Node.js** - JavaScript runtime environment
- **Mongoose** - MongoDB ODM for Node.js

## Prerequisites
Before you begin, ensure you have met the following requirements:
- You have installed **Node.js** and **npm**.
- You have a MongoDB instance running (either locally or via MongoDB Atlas).

## Installation

### 1. Clone the Repository

git clone https://github.com/aj27sargar/Connection-of-MERN.git
2. Install Dependencies
Navigate into the cloned project directory and install the necessary dependencies for both the backend and frontend:

bash
Copy code
# Install backend dependencies
cd backend
npm install

# Install frontend dependencies
cd ../frontend
npm install
3. Set Up MongoDB
Make sure MongoDB is running on your system or use MongoDB Atlas. If using Atlas, make sure to obtain your connection URI.

Running the Application
1. Backend
Navigate to the backend folder and run the backend server using:

bash
Copy code
cd backend
npm start
By default, the backend will run on http://localhost:5000.

2. Frontend
Navigate to the frontend folder and run the React frontend:

bash
Copy code
cd ../frontend
npm start
By default, the frontend will run on http://localhost:3000.

Environment Variables
To connect to your MongoDB instance, create a .env file in the backend directory with the following content:

env
Copy code
MONGO_URI=mongodb+srv://<username>:<password>@cluster0.mongodb.net/<dbname>?retryWrites=true&w=majority
Replace <username>, <password>, and <dbname> with your MongoDB credentials.

Project Structure
The basic structure of the project is as follows:

bash
Copy code
Connection-of-MERN/
│
├── backend/
│   ├── models/        # Mongoose models
│   ├── routes/        # Express routes         
│   ├── index.js      # Express server
│   └── .env           # Environment variables for MongoDB
│
├── frontend/
│   ├── src/           # React source files
│   ├── public/        # Public static files
│   └── package.json   # Frontend dependencies
Usage
Once both backend and frontend servers are running, you can use the application by navigating to http://localhost:3000 in your browser.

Contributing
Contributions are welcome! Please feel free to submit a Pull Request or open an Issue.

License
This project is licensed under the MIT License.
