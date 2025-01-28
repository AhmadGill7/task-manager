# Task Manager Application

A full-stack task management application built with React, Node.js, and MySQL.

## Features

- User authentication (Register/Login)
- Create, read, update, and delete tasks
- Protected routes and API endpoints
- Modern UI with Material-UI components
- State management with Redux Toolkit
- Real-time updates

## Tech Stack

### Frontend

- React
- Redux Toolkit
- Material-UI
- React Router
- Axios
- Vite

### Backend

- Node.js
- Express
- MySQL
- Sequelize ORM
- JWT Authentication
- bcrypt for password hashing

## Prerequisites

- Node.js (v18 or higher)
- MySQL
- PNPM package manager

## Getting Started

1. **Clone the repository**

`bash git clone <repository-url>`

2. **Database Setup**

- Create a MySQL database named "task_manager"
- Configure your database connection in server/.env

3. **Environment Variables**

Create .env files in both client and server directories:

Server (.env):

```
PORT=5000
DB_NAME=task_manager
DB_USER=your_username
DB_PASSWORD=your_password
DB_HOST=localhost
JWT_SECRET=your_jwt_secret
```

Client (.env):

```
VITE_API_URL=http://localhost:5000/api
```

4. **Install Dependencies**

```
For the backend: cd server && pnpm install
For the frontend: cd client && pnpm install
```

5. **Start the Development Servers**

```
For the backend: cd server && pnpm dev
For the frontend: cd client && pnpm dev
```

6. **Access the Application**

Open your browser and navigate to `http://localhost:5173` to access the application.

## Project Structure

```
task-manager/
├── client/ # Frontend React application
│ ├── src/
│ │ ├── components/ # Reusable components
│ │ ├── features/ # Redux slices and logic
│ │ ├── pages/ # Page components
│ │ ├── services/ # API services
│ │ └── app/ # Redux store setup
│ └── ...
├── server/ # Backend Node.js application
│ ├── src/
│ │ ├── config/ # Database configuration
│ │ ├── controllers/ # Route controllers
│ │ ├── middlewares/ # Custom middlewares
│ │ ├── models/ # Database models
│ │ └── routes/ # API routes
│ └── ...
└── README.md
```


## API Endpoints

### Authentication
- POST `/api/auth/register` - Register a new user
- POST `/api/auth/login` - Login user

### Tasks
- GET `/api/tasks` - Get all tasks for authenticated user
- POST `/api/tasks` - Create a new task
- PUT `/api/tasks/:id` - Update a task
- DELETE `/api/tasks/:id` - Delete a task

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

Contributions are welcome! Please feel free to submit a pull request.

## License

This project is open-sourced under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Thanks to the React, Node.js, and MySQL communities for their amazing libraries and tools.
- Special thanks to the contributors of the libraries and tools used in this project.
