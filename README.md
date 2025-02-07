🌐 SMPP Web Portal

📖 Overview

This project is an SMPP (Short Message Peer-to-Peer) Web Portal that provides a REST API for managing SMPP connections, sending messages, conducting load tests, and logging activities. The backend is built using Node.js and Express, with MongoDB as the database. JWT authentication is implemented for security.

📸 Screenshots

![smpp1](https://github.com/user-attachments/assets/b8a99f49-d285-47c5-89bf-44942fc039bb)
![smpp1-config](https://github.com/user-attachments/assets/dda14130-9d28-4013-ae6e-e7d854229094)
![smpp1-loadtest](https://github.com/user-attachments/assets/7977c006-c3ef-40ae-bd8a-e31dfc671d5d)
![smpp1-message](https://github.com/user-attachments/assets/51e80978-f6d2-44e7-a7ed-acd6cb257932)



✨ Features

🔐 User Authentication

Register and login with JWT authentication

🔌 SMPP Connection Management

Connect and disconnect from an SMPP server

Support for TX (transmitter) and RX (receiver) modes

📩 Message Sending

Send messages via SMPP

Submit messages through a REST API

🚀 Load Testing

Perform SMPP load tests

Abort ongoing load tests

⚙️ Configuration Management

Save and retrieve SMPP configurations

📜 Logging

Retrieve logs related to SMPP activities

🛠️ Technologies Used

Backend: Node.js, Express

Database: MongoDB

Authentication: JWT

Services: SMPP (via smppService)

🔗 API Endpoints

🔑 Authentication

POST /api/register - Register a new user

POST /api/login - Authenticate user and get JWT token

⚙️ Configuration

POST /api/saveconfig - Save SMPP configuration (Requires authentication)

GET /api/getconfig - Retrieve SMPP configuration (Requires authentication)

📜 Logging

GET /api/getlog - Get system logs (Requires authentication)

🔌 SMPP Management

POST /api/connectsmpp - Connect to SMPP server (Requires authentication)

POST /api/disconnectsmpp - Disconnect from SMPP server (Requires authentication)

POST /api/txonlysmpp - Set SMPP to TX (transmitter) mode (Requires authentication)

POST /api/rxonlysmpp - Set SMPP to RX (receiver) mode (Requires authentication)

GET /api/smppConnection - Get SMPP connection status

✉️ Messaging

POST /api/send-message - Send an SMPP message (Requires authentication)

POST /api/submit-message - Submit a message through the REST API (Requires authentication)

🚀 Load Testing

POST /api/loadtest - Start an SMPP load test (Requires authentication)

POST /api/abortloadtest - Abort an ongoing SMPP load test (Requires authentication)

🛠️ Installation

📌 Prerequisites

Node.js (v16 or later recommended)

MongoDB

An SMPP server

📥 Setup

1️⃣ Clone the repository:

git clone <repository_url>
cd <project_directory>

2️⃣ Install dependencies:

npm install

3️⃣ Set up environment variables:

Create a .env file in the project root with the following variables:

MONGODB_URI=<your_mongodb_connection_string>
JWT_SECRET=<your_jwt_secret>
PORT=3004

4️⃣ Start the server:

npm start

🚀 Usage

Use Postman or a frontend application to interact with the API.

Authenticate using JWT for protected endpoints.

📜 Logging

Logs are managed through the logger utility and stored in MongoDB.

📜 License

This project is for internal use and is not publicly licensed.



