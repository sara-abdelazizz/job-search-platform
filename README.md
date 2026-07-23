# 💼 Job Search Platform API

A scalable backend application built with **NestJS** and **TypeScript** that connects job seekers with companies. The platform provides secure authentication, job management, application tracking, real-time messaging, notifications, and an admin dashboard.

---

## 🚀 Features

### 🔐 Authentication & Authorization
- User & Company Registration
- Secure Login
- Google Authentication
- Email Verification with OTP
- Password Reset
- JWT Authentication
- Role-Based Authorization (Admin, Company, User)

### 👤 User Management
- Update Profile
- Change Password
- Restore Account
- Browse Jobs
- Search Jobs
- Apply for Jobs
- View Application History

### 🏢 Company Management
- Create Company Profile
- Update Company Information
- Add Job Opportunities
- Update Job Posts
- Delete Job Posts
- View Company Jobs
- Manage Applicants

### 💼 Job Management
- Create Jobs
- Update Jobs
- Delete Jobs
- Get Company Jobs
- Search & Filter Jobs
- View Job Details

### 📄 Applications
- Apply for Jobs
- Update Application Status
- Retrieve Applications

### 💬 Real-Time Chat
- One-to-One Messaging
- Chat History
- WebSocket Communication

### 🔔 Notifications
- Real-Time Notifications
- Socket.IO Gateway

### 👨‍💼 Admin Dashboard
- Manage Users
- Manage Companies
- Manage Jobs
- Manage Applications
- GraphQL Support

---

# 🛠️ Tech Stack

- **TypeScript**
- **NestJS**
- **MongoDB**
- **Mongoose**
- **GraphQL**
- **Apollo Server**
- **Socket.IO**
- **JWT**
- **Passport.js**
- **bcrypt**
- **Nodemailer**
- **Multer**
- **Cron Jobs**

---

# 📂 Project Structure

```text
src/
├── DB/
│   └── Models/
│       ├── applications.model.ts
│       ├── chat.model.ts
│       ├── company.model.ts
│       ├── job.model.ts
│       ├── otp.model.ts
│       └── user.model.ts
│
├── admin/
├── applications/
├── auth/
├── chat/
├── company/
├── jobs/
├── notifications/
├── user/
│
├── common/
│   ├── sockets/
│   ├── crons/
│   ├── enums/
│   ├── guards/
│   ├── hashing/
│   ├── interceptors/
│   ├── multer/
│   ├── pipes/
│   ├── services/
│   └── utils/
│
├── app.module.ts
├── app.controller.ts
├── app.service.ts
├── main.ts
└── schema.gql

test/

package.json
tsconfig.json
```

---

# 📡 REST API Modules

| Module | Description |
|---------|-------------|
| Auth | Authentication & Authorization |
| User | User Profile Management |
| Company | Company Management |
| Jobs | Job CRUD Operations |
| Applications | Job Applications |
| Chat | Real-Time Messaging |
| Notifications | Socket Notifications |
| Admin | Dashboard & GraphQL |

---

# ⚙️ Installation

Clone the repository

```bash
git clone https://github.com/sara-abdelazizz/job-search-platform
```

Navigate to the project

```bash
cd job-search-platform
```

Install dependencies

```bash
npm install
```

Create a `.env` file

```env
PORT=

DB_URI=

SALT=
SALT_ROUNDS=

TOKEN_ACCESS_ADMIN_SECRET=
TOKEN_REFRESH_ADMIN_SECRET=
TOKEN_ACCESS_USER_SECRET=
TOKEN_REFRESH_USER_SECRET=

ACCESS_TOKEN_EXPIRE_IN=
REFRESH_TOKEN_EXPIRE_IN=
OTP_EXPIRE_IN=

EMAIL=
PASS=

ENCRYPTION_KEY=
IV_LENGTH=

CLOUD_NAME=
API_KEY=
API_SECRET=
```

Run the development server

```bash
npm run start:dev
```

---

# 🔒 Security

- JWT Authentication
- Role-Based Access Control (RBAC)
- Password Hashing with bcrypt
- DTO Validation using ValidationPipe
- Global Exception Handling
- Environment Variables
- Secure File Upload Validation

---

# 🧪 Testing

Both REST APIs and GraphQL operations were tested using **Postman**.

---

# 📌 Future Improvements

- Docker Support
- CI/CD Pipeline
- Unit & Integration Testing
- API Documentation with Swagger
- Redis Caching
- Microservices Architecture

---

# 👩‍💻 Author

**Sara Abdelaziz**

Backend Developer

- GitHub: https://github.com/sara-abdelazizz
- LinkedIn: https://www.linkedin.com/in/sara-abdelaziz-9722b22a7/

---

# 📄 License

This project was built for learning and portfolio purposes.
