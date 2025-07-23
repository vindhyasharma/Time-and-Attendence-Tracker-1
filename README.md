# 🚀 MERN Stack Time & Attendance Tracking System

A comprehensive employee time and attendance tracking system built with the **pure MERN Stack** (MongoDB, Express.js, React.js, Node.js) in **JavaScript**.

## 🏗️ Pure MERN Architecture

\`\`\`
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   Frontend      │◄──►│    Backend      │◄──►│    Database     │
│   React.js      │    │   Express.js    │    │    MongoDB      │
│   (JavaScript)  │    │   Node.js       │    │   (Mongoose)    │
│                 │    │   (JavaScript)  │    │                 │
└─────────────────┘    └─────────────────┘    └─────────────────┘
\`\`\`

## 🎯 Tech Stack

- **M**ongoDB - NoSQL Database with Mongoose ODM
- **E**xpress.js - Web Application Framework for Node.js
- **R**eact.js - Frontend Library with Context API
- **N**ode.js - JavaScript Runtime Environment

## 📁 Project Structure

\`\`\`
mern-attendance-system/
├── server/                 # Express.js Backend (JavaScript)
│   ├── models/            # Mongoose Models
│   │   ├── Employee.js
│   │   ├── Attendance.js
│   │   └── Leave.js
│   ├── routes/            # API Routes
│   │   ├── auth.js
│   │   ├── employees.js
│   │   ├── attendance.js
│   │   └── leaves.js
│   ├── middleware/        # Custom Middleware
│   │   └── auth.js
│   ├── server.js          # Entry Point
│   └── package.json
├── client/                # React.js Frontend (JavaScript)
│   ├── src/
│   │   ├── components/    # React Components
│   │   ├── pages/         # Page Components
│   │   ├── contexts/      # Context API
│   │   ├── services/      # API Services
│   │   └── App.js
│   └── package.json
└── scripts/               # Utility Scripts
    └── init-sample-data.js
\`\`\`

## 🚀 Quick Start

### 1. Clone Repository
\`\`\`bash
git clone <repository-url>
cd mern-attendance-system
\`\`\`

### 2. Backend Setup
\`\`\`bash
cd server
npm install
cp .env.example .env
# Configure MongoDB URI in .env file
npm run dev
\`\`\`

### 3. Frontend Setup
\`\`\`bash
cd client
npm install
npm start
\`\`\`

### 4. Initialize Sample Data
\`\`\`bash
cd scripts
node init-sample-data.js
\`\`\`

## 🔐 Demo Credentials

| Role | Email | Password |
|------|-------|----------|
| **Admin** | admin@company.com | admin123 |
| **Manager** | jane.smith@company.com | password123 |
| **Employee** | john.doe@company.com | password123 |

## ✨ Features

### 🔐 Authentication & Authorization
- JWT-based authentication
- Role-based access control (Admin, Manager, Employee)
- Secure password hashing with bcrypt

### ⏰ Time Tracking
- Real-time clock in/out functionality
- Break management system
- Location tracking
- Automatic overtime calculation

### 📊 Attendance Management
- Daily attendance records
- Status tracking (Present, Late, Absent)
- Attendance history and reports
- Monthly statistics

### 🏖️ Leave Management
- Leave request submission
- Approval/rejection workflow
- Leave balance tracking
- Multiple leave types (Annual, Sick, Personal, Emergency)

### 👥 Employee Management
- Employee CRUD operations
- Department and role management
- Profile management
- Employee statistics

### 📈 Reports & Analytics
- Attendance reports
- Department-wise statistics
- Employee performance metrics
- Data visualization

### 📱 User Interface
- Responsive design for all devices
- Modern and intuitive UI
- Real-time updates
- Toast notifications

## 🛠️ API Endpoints

### Authentication
- `POST /api/auth/login` - User login
- `POST /api/auth/register` - User registration
- `GET /api/auth/me` - Get current user

### Employees
- `GET /api/employees` - Get all employees
- `POST /api/employees` - Create employee
- `PUT /api/employees/:id` - Update employee
- `DELETE /api/employees/:id` - Delete employee

### Attendance
- `POST /api/attendance/clock-in` - Clock in
- `POST /api/attendance/clock-out` - Clock out
- `GET /api/attendance` - Get attendance records
- `POST /api/attendance/break` - Manage breaks

### Leaves
- `POST /api/leaves` - Apply for leave
- `GET /api/leaves` - Get leave requests
- `PATCH /api/leaves/:id/status` - Approve/reject leave

## 🔧 Environment Variables

### Backend (.env)
\`\`\`env
MONGODB_URI=mongodb://localhost:27017/attendance_system
JWT_SECRET=your_super_secret_jwt_key
PORT=5000
NODE_ENV=development
\`\`\`

### Frontend (.env)
\`\`\`env
REACT_APP_API_URL=http://localhost:5000/api
\`\`\`

## 🚀 Deployment

### Backend Deployment
1. Deploy to platforms like Heroku, Railway, or DigitalOcean
2. Set environment variables
3. Connect to MongoDB Atlas for production database

### Frontend Deployment
1. Build the React app: `npm run build`
2. Deploy to Netlify, Vercel, or any static hosting service
3. Update API URL for production

## 🧪 Testing

\`\`\`bash
# Backend tests
cd server
npm test

# Frontend tests
cd client
npm test
\`\`\`

## 📝 License

This project is licensed under the MIT License.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## 📞 Support

For support and questions, please open an issue in the repository.

---

**Built with ❤️ using the MERN Stack**
