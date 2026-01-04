

````markdown
# Student Attendance System

![GitHub repo size](https://img.shields.io/github/repo-size/helaluddin-swe/react-basics)
![GitHub contributors](https://img.shields.io/github/contributors/helaluddin-swe/react-basics)
![GitHub stars](https://img.shields.io/github/stars/helaluddin-swe/react-basics?style=social)
![GitHub license](https://img.shields.io/github/license/helaluddin-swe/react-basics)



A **full-stack web application** for managing student attendance efficiently.  
It allows students to mark attendance, and admins to manage and track attendance records in real-time.

---

## 🚀 Features
- **Student login and authentication**: Secure login for students.  
- **Attendance tracking**: Students can mark attendance; admins can view and manage attendance records.  
- **Admin dashboard**: Manage students, view reports, and monitor attendance.  
- **Responsive design**: Works on both desktop and mobile devices.  
- **React Hooks**: Functional components using `useState` and other hooks for state management.

---

## 🛠 Tech Stack
- **Frontend:** React (with Hooks, Context API)  
- **Backend:** Node.js, Express  
- **Database:** MongoDB  
- **Authentication:** JWT (JSON Web Tokens)  
- **Styling:** CSS / Tailwind CSS (optional)  

---

## ⚛️ React Hooks Usage

This project uses **React Hooks** for state management and functional components.  

### Example: `useState`
```javascript
import React, { useState } from 'react';

function AttendanceCounter() {
  // useState hook to manage attendance count
  const [count, setCount] = useState(0);

  const markAttendance = () => {
    setCount(count + 1);
  };

  return (
    <div>
      <h2>Attendance Count: {count}</h2>
      <button onClick={markAttendance}>Mark Attendance</button>
    </div>
  );
}

export default AttendanceCounter;
````

### Explanation

* `useState` allows **functional components** to maintain state.
* `count` stores the current attendance count.
* `setCount` updates the count when a student marks attendance.
* Using Hooks makes the code **cleaner and easier to maintain** than class components.
* Other hooks like `useEffect` are used for **fetching data and updating the UI dynamically**.

---

## 📂 Folder Structure

```
student-attendance-system/
├─ backend/
│  ├─ models/           # Mongoose models
│  ├─ routes/           # API routes
│  ├─ controllers/      # Route handlers
│  ├─ config/           # DB connection and environment config
│  └─ server.js         # Express server
├─ frontend/
│  ├─ src/
│  │  ├─ components/    # Reusable UI components
│  │  ├─ pages/         # Pages like Login, Dashboard
│  │  ├─ context/       # React Context API
│  │  └─ App.js
├─ package.json
└─ README.md
```

---

## 🔗 API Endpoints

### Auth

* `POST /api/auth/login` → Login student/admin
* `POST /api/auth/register` → Register student/admin

### Attendance

* `GET /api/attendance` → Get all attendance records
* `POST /api/attendance` → Mark attendance
* `PUT /api/attendance/:id` → Update attendance
* `DELETE /api/attendance/:id` → Delete attendance record

> **Note:** Protected routes require JWT token authentication.

---

## 📦 Installation

Follow these steps to set up the project locally:

```bash
# Clone the repository
git clone https://github.com/helaluddin-swe/react-basics.git

# Navigate into the project directory
cd react-basics

# Install backend dependencies
cd backend
npm install

# Start backend server
npm run dev

# Install frontend dependencies
cd ../frontend
npm install

# Start frontend server
npm start
```

---

## ⚡ Usage

* Students can **log in** and **mark attendance**.
* Admins can **view, edit, and delete** attendance records.
* Dashboard provides **summary reports** of attendance.

---

## 📝 Contribution

Contributions are welcome!

1. Fork the repository
2. Create a new branch: `git checkout -b feature-name`
3. Make changes and commit: `git commit -m "Add feature"`
4. Push to the branch: `git push origin feature-name`
5. Create a Pull Request

---

## 🔗 Links

* **GitHub Repository:** [Click here to view the source code](https://github.com/helaluddin-swe/react-basics)
* **Live Demo:** [Click here to view the live project](#) <!-- Replace # with your live link -->

---

## 📜 License

This project is licensed under the **MIT License**.

---

## 🎯 Future Improvements

* Add **email notifications** for attendance alerts.
* Add **role-based access control**.
* Add **export/import attendance records** (CSV, PDF).
* Implement **analytics dashboard** with charts and stats.

```

