# Admin Login System

A full-stack web application for user management with different membership types and admin capabilities.

## Features

- User registration with membership types
- User authentication and authorization
- Admin dashboard for user management
- Module enrollment system
- Password management
- Role-based access control

## Tech Stack

- Frontend: React.js
- Backend: Node.js with Express
- Database: MySQL
- Authentication: JWT with HTTP-only cookies

## Prerequisites

- Node.js (v14 or higher)
- MySQL Server
- npm or yarn

## Installation

1. Clone the repository:
```bash
git clone <your-repository-url>
cd admin-login
```

2. Install dependencies:
```bash
# Install backend dependencies
cd Server
npm install

# Install frontend dependencies
cd ../client2
npm install
```

3. Set up the database:
- Create a MySQL database named 'mydb'
- The tables will be created automatically when you start the server

4. Create a .env file in the Server directory:
```
SECRET_KEY=your_secret_key
```

## Running the Application

1. Start the backend server:
```bash
cd Server
npm start
```

2. Start the frontend development server:
```bash
cd client2
npm start
```

The application will be available at:
- Frontend: http://localhost:3001
- Backend: http://localhost:5000

## Project Structure

```
admin-login/
├── Server/             # Backend server code
│   ├── server.js      # Main server file
│   └── package.json   # Backend dependencies
├── client2/           # Frontend React application
│   ├── src/          # Source code
│   └── package.json  # Frontend dependencies
└── README.md         # Project documentation
```

## API Endpoints

- POST /signup - Register a new user
- POST /login - User login
- GET /me - Get current user data
- POST /logout - User logout
- GET /all-users - Get all users (admin only)
- POST /toggle-admin - Toggle admin status (admin only)
- POST /change-password - Change user password
- GET /user/modules - Get user's enrolled modules
- POST /user/enroll-module - Enroll in a module

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details. 