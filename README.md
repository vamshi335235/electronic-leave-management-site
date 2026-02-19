# 📋 Electronic Leave Management System (ELMS)

A robust, enterprise-grade web application designed to streamline the leave application and approval process for educational institutions. This system provides a seamless interface for students to apply for leaves and for Heads of Departments (HOD) to manage and monitor them efficiently.

---

## 🚀 Features

### 👨‍🎓 Student Portal
- **Dashboard**: Real-time overview of leave status and statistics.
- **Leave Application**: Easy-to-use form to submit leave requests.
- **Leave History**: Comprehensive view of all past and current leave applications.
- **Calendar Integration**: Visual representation of academic schedules and leaves.
- **Notifications**: Instant updates on leave approval or rejection.
- **Profile Management**: Update personal information and academic details.
- **Chat System**: Interactive communication channel.

### 👨‍💼 HOD (Head of Department) Portal
- **Consolidated Dashboard**: High-level statistics of departmental leave activities.
- **Leave Management**: Review, approve, or reject pending leave requests with comments.
- **Student Management**: Capability to add and manage student records.
- **Reporting**: Generate detailed reports of leave patterns and student attendance.
- **Departmental Calendar**: Track all departmental leaves in a unified calendar view.
- **Automatic Notifications**: Send automated alerts to students regarding their application status.

---

## 🛠️ Tech Stack

- **Frontend**: HTML5, CSS3, JavaScript, Bootstrap (Assets-based)
- **Backend**: PHP (Modular Architecture)
- **Database**: MySQL
- **Tooling**: Git version control

---

## 📁 Project Structure

```text
├── HOD/               # Head of Department modules & dashboard
├── student/           # Student portal modules & dashboard
├── auth/              # Authentication (Login/Logout) logic
├── sql/               # Database schema and SQL dumps
├── assets/            # Static files (CSS, JS, Images)
├── db.php             # Database connection configuration
├── index.php          # Main entry point/Routing
└── loader.html        # Preloader component
```

---

## ⚙️ Setup Instructions

### Prerequisites
- Local Server Environment (XAMPP, WAMP, or MAMP)
- PHP 7.4 or higher
- MySQL Database

### Installation Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/vamshi335235/electronic-leave-management-site.git
   cd electronic-leave-management-site
   ```

2. **Database Setup**
   - Open PHPMyAdmin.
   - Create a new database named `lmsbtech`.
   - Import the SQL files located in the `sql/` directory:
     - `lmsbtech_user.sql`
     - `lmsbtech_leaves.sql`
     - `lmsbtech_notifications.sql`

3. **Configure Database Connection**
   - Open `db.php`.
   - Update the database credentials to match your local setup:
     ```php
     $sname = "localhost";
     $uname = "root";
     $password = ""; // Your MySQL password
     $db_name = "lmsbtech";
     ```

4. **Run the Application**
   - Move the project folder to your server's root directory (e.g., `htdocs` for XAMPP).
   - Access the application at `http://localhost/electronic-leave-management-site`.

---

## 🔐 Default Roles
The system supports two primary roles:
- **Student**: Can apply for leaves and track progress.
- **HOD**: Can manage approvals and department records.

---

## 📄 License
This project is part of a major academic submission. All rights reserved.

---

*Built with ❤️ for efficient campus management.*