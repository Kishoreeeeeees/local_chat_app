# Local Chat Application using MERN Stack

## Project Overview
This project aims to create a local chat application allowing multiple users on the same device to communicate in different chat rooms. The backend handles user authentication, message storage, and room management. It uses Node.js for the backend server, MongoDB for database storage, and React for the frontend interface.

### Key Features
- Multi-room chat capabilities with user-specific access.
- Real-time messaging within the local network.
- User registration and login with hashed passwords.
- Persistent message storage with the ability to retrieve history on login.

### Technical Specifications
- **Backend**: Node.js with Express.js for RESTful API development.
- **Database**: MongoDB for storing user data, rooms, and messages.
- **Frontend**: React for building the user interface.
- **Authentication**: JWT (JSON Web Tokens) for secure user authentication and session management.
- **Real-time Communication**: Socket.io for real-time messaging between clients.
- **Development Environment**: Electron for packaging the application for local deployment.

## Prerequisites
Before running the application, ensure you have the following installed:
- Node.js and npm (Node Package Manager)
- MongoDB (running locally or on a network accessible server)
- React.js (for frontend development)
- Electron (for local desktop application)

## Installation and Setup
### Backend Setup (Node.js + Express.js)
1. Clone the repository:
   ```bash
   git clone <repository_url>
   cd local-chat-app/backend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up environment variables:
   - Create a `.env` file in the `backend` directory.
   - Define environment variables:
     ```plaintext
     PORT=5000
     MONGODB_URI=mongodb://localhost:27017/local_chat_app
     JWT_SECRET=your_jwt_secret
     ```

4. Start the backend server:
   ```bash
   npm start
   ```

### Frontend Setup (React.js)
1. Navigate to the frontend directory:
   ```bash
   cd ../frontend
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the React development server:
   ```bash
   npm start
   ```

### Electron Setup (for packaging as a desktop application)
1. Install Electron globally (if not already installed):
   ```bash
   npm install -g electron
   ```

2. Build the React frontend for Electron:
   ```bash
   npm run build
   ```

3. Start Electron:
   ```bash
   electron .
   ```

## Usage
1. Register and log in with your credentials.
2. Create or join chat rooms.
3. Start chatting with other users in real-time.
4. Messages are stored locally and can be retrieved on subsequent logins.

## Contributing
Contributions are welcome! Please follow these guidelines:
- Fork the repository and create your branch (`git checkout -b feature/YourFeature`).
- Commit your changes (`git commit -am 'Add some feature'`).
- Push to the branch (`git push origin feature/YourFeature`).
- Create a new Pull Request.

## License
This project is licensed under the [MIT License](LICENSE).

## Acknowledgements
- Thanks to [Socket.io](https://socket.io/) for real-time communication.
- Inspiration from similar projects and open-source contributions.

---

This README provides a comprehensive guide for setting up, using, and contributing to the local chat application using the MERN stack. Adjust paths and specifics as per your actual project structure and requirements.
