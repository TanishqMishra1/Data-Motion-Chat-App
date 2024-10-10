# Data-Motion-Chat-App

This project is a real-time chat application that allows multiple users to join, send, and receive messages instantly. The application uses WebSockets for real-time messaging and supports multiple users in a chat room. It also implements user authentication and stores chat history in a database.

Table of Contents
1.Overview
2.Features
3.Technologies
4.Setup
5.Usage
6.Database
7.Scalability
8.Contributing
9.License


1.Overview
This project focuses on building a full-stack real-time chat application using JavaScript, ensuring instant messaging with WebSockets and managing user authentication using JWT. The application is built with the following architecture:

Frontend: React.js (using Vite for bundling).
Backend: Node.js with Express.
Database: MongoDB for storing user data and chat history.

2.Features
Real-Time Messaging:

WebSocket connections are used for real-time messaging between users.
Supports multiple users in the same chat room.
Messages appear instantly in the chat window without page reloads.
User Authentication:

JWT-based user authentication.
Each user has a unique username or identifier in the chat room.
Non-authenticated users cannot access the chat room.
Frontend:

Built using React.js with Vite for web.
Chat interface displays:
List of users in the chat room.
Chat window with messages and timestamps.
Input form to send messages.
New users joining are dynamically added to the user list.
Backend:

Uses WebSockets for real-time message exchanges.
REST API endpoints handle user authentication and other non-real-time interactions.
Built with Node.js and Express.
Database:

Persistent data storage using MongoDB for users and chat history.




3.Technologies
Frontend: React.js, Vite
Backend: Node.js, Express
Database: MongoDB
Authentication: JWT
Real-Time Communication: WebSockets




4.Setup
Prerequisites
Make sure you have the following installed:

Node.js (v14+)
MongoDB (local or cloud instance)
Installation
Clone the repository:

bash
Copy code
git clone git remote add origin https://github.com/TanishqMishra1/DataMotion-ChatApp.git
Navigate to the project directory:

bash
Copy code
cd real-time-chat-app
Install dependencies for both frontend and backend:

bash
Copy code
# Navigate to backend folder and install dependencies
cd backend
npm install

# Navigate to frontend folder and install dependencies
cd ../frontend
npm install
Set up environment variables:

In the backend directory, create a .env file and add the following variables:
bash
Copy code
MONGO_URI=your-mongodb-uri
JWT_SECRET=your-secret-key
Start the backend server:

bash
Copy code
cd backend
npm start
Start the frontend server:

bash
Copy code
cd frontend
npm run dev





5.Usage
Open your browser and navigate to http://localhost:5173 to access the chat application.
Log in or sign up to join the chat.
Start sending and receiving real-time messages in a chat room with other users.
Scripts
Backend:
npm start - Starts the backend server.
Frontend:
npm run dev - Starts the frontend in development mode with hot-reloading.





6.Database
The application uses MongoDB as a persistent database to store user data and chat history. The reason for choosing MongoDB (a non-relational database) is due to its flexibility with storing documents like user profiles and chat messages, which can vary in structure. Additionally, MongoDB’s scalability makes it suitable for high volumes of chat messages.

MongoDB vs. SQL:
MongoDB offers flexible schema design and is optimized for high-throughput applications.
SQL (e.g., PostgreSQL) could be used for stricter relational data handling, but MongoDB's document-based model is more efficient for handling real-time data like chat messages.





7.Scalability
This chat application is designed to be scalable with the following considerations:

WebSocket Management: WebSockets handle real-time connections efficiently. In production, load balancing WebSocket connections across multiple instances can be done using tools like Nginx or cloud services.
Database: MongoDB scales horizontally and can handle large volumes of chat data across distributed servers.
Cloud Deployment: The app can be deployed to cloud providers like AWS, Azure, or DigitalOcean, ensuring high availability and scalability.





8.Contributing
Contributions are welcome! Please fork this repository, make your changes in a new branch, and submit a pull request for review.

Fork the repository.
Create a new branch (git checkout -b feature-name).
Commit your changes (git commit -m 'Add feature').
Push to the branch (git push origin feature-name).
Open a Pull Request.





9.License
This project is licensed under the MIT License. See the LICENSE file for details.




<!-- Demo User -->
Email- ivar@gmail.com   
Password - demo1234

<!-- Demo User-2 -->
Email - jon@gmail.com
Password - demo1234
