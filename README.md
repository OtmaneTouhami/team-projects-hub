# Projects Management System

A comprehensive project management platform designed for team collaboration, task tracking, and workspace management.

## 📋 About

This project management system is a collaborative platform built as part of the Web Technologies course for the Master's Degree in Distributed Systems and Artificial Intelligence at ENSET El Mohammadia. It enables teams to organize their work using workspaces, projects, and tasks with role-based access control.

### Key Features

- **User Authentication**: Secure login and registration with local credentials and Google OAuth
- **Workspaces**: Create and manage separate workspaces for different teams/organizations
- **Projects**: Organize work into projects within workspaces
- **Task Management**: Create, assign, track, and update tasks
- **Role-Based Permissions**: Control access with customizable user roles
- **Real-time Collaboration**: Team members can work together seamlessly
- **Modern UI**: Responsive and intuitive user interface using React and Shadcn UI components

## 🚀 Technologies Used

### Backend

- Node.js & Express
- TypeScript
- MongoDB with Mongoose
- Passport.js for authentication
- Zod for validation
- RESTful API architecture

### Frontend

- React with TypeScript
- Vite as build tool
- React Query for data fetching
- React Router for navigation
- Shadcn UI components with Tailwind CSS
- Context API for state management

## 🛠️ Setup Instructions

### Prerequisites

- Node.js (v16 or higher)
- MongoDB
- pnpm package manager

### Environment Configuration

1. Clone the repository:

```bash
git clone <repository-url>
cd projects-management
```

2. Backend Setup:

```bash
cd backend
# Create a .env file with the following variables
echo "PORT=5000
MONGO_URI=mongodb://localhost:27017/projects-management
JWT_SECRET=your_jwt_secret_key
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret
CLIENT_URL=http://localhost:3000
BASE_PATH=/api/v1
NODE_ENV=development" > .env

# Install dependencies
pnpm install

# Seed initial roles data
pnpm seed

# Start development server
pnpm dev
```

3. Frontend Setup:

```bash
cd ../client
# Create a .env file if needed
echo "VITE_API_URL=http://localhost:5000/api/v1" > .env

# Install dependencies
pnpm install

# Start development server
pnpm dev
```

4. Access the application:
   - Frontend: http://localhost:3000
   - Backend API: http://localhost:5000/api/v1

## 🗂️ Project Structure

### Backend

```
backend/
├── src/
│   ├── @types/            # TypeScript type definitions
│   ├── config/            # Application configuration
│   ├── controllers/       # Route controllers
│   ├── enums/             # TypeScript enums
│   ├── middlewares/       # Express middlewares
│   ├── models/            # Mongoose models
│   ├── routes/            # API routes
│   ├── seeders/           # Database seeders
│   ├── services/          # Business logic
│   ├── utils/             # Utility functions
│   ├── validation/        # Request validation
│   └── index.ts           # Application entry point
```

### Frontend

```
client/
├── public/               # Static files
├── src/
│   ├── assets/           # Images and other assets
│   ├── components/       # Reusable UI components
│   ├── constant/         # Constants and configurations
│   ├── context/          # React contexts
│   ├── hooks/            # Custom React hooks
│   ├── layout/           # Layout components
│   ├── lib/              # Utility libraries
│   ├── pages/            # Application pages
│   ├── routes/           # Route configurations
│   └── types/            # TypeScript type definitions
```

## 👥 Team Members

- Yassir JERAIDI
- Mohamed HAKIM
- Rim AALOI
- Otmane TOUHAMI

## 📄 License

This project is part of academic coursework for ENSET El Mohammadia and is not licensed for commercial use.

---

Developed with ❤️ for Web Technologies course - Master's in Distributed Systems and Artificial Intelligence
