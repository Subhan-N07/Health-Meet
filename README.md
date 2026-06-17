# 🏥 Health-Meet

[![GitHub stars](https://img.shields.io/github/stars/Subhan-N07/Health-Meet?style=for-the-badge&color=4169E1)](https://github.com/Subhan-N07/Health-Meet/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/Subhan-N07/Health-Meet?style=for-the-badge&color=00BFFF)](https://github.com/Subhan-N07/Health-Meet/network/members)
[![Issues](https://img.shields.io/github/issues/Subhan-N07/Health-Meet?style=for-the-badge&color=FF4500)](https://github.com/Subhan-N07/Health-Meet/issues)
[![MIT License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](LICENSE)

**Health-Meet** is a comprehensive, feature-rich full-stack medical appointment scheduling platform built to streamline interactions between patients, doctors, and healthcare administrators. Featuring role-based dashboards, secure authentications, dynamic booking flows, and real-time appointment tracking, Health-Meet ensures hassle-free healthcare coordination.

---

## 📸 Interface Preview

> 💡 **Note:** To render these screenshots correctly on GitHub, make sure to add these image files to an assets/screenshots directory in your repository or adjust the image paths to point to where you host them.

### 🌐 Patient Portal

| 🏠 Landing Page (`User Interface.jpg`) | 🔍 Doctor Discovery (`Available Doctor Interface.jpg`) |
| :---: | :---: |
| <img src="User Interface.jpg" width="100%" alt="Landing Page"/> | <img src="Available Doctor Interface.jpg" width="100%" alt="Available Doctors"/> |

| 📅 Booking Calendar (`Slot and Time Booking Interface.png`) | 💳 Booking Status (`Online Payment Interface.png`) |
| :---: | :---: |
| <img src="Slot and Time Booking Interface.png" width="100%" alt="Slot and Time Booking"/> | <img src="Online Payment Interface.png" width="100%" alt="Razorpay Status"/> |

| 🕒 Appointment History (`Appointment Booking and Cancel Interface.png`) | 👤 Profile Management (`Patient Profile Interface.png`) |
| :---: | :---: |
| <img src="Appointment Booking and Cancel Interface.png" width="100%" alt="Appointments Status"/> | <img src="Patient Profile Interface.png" width="100%" alt="Patient Profile"/> |

### 🩺 Doctor Dashboard

| 📊 Doctor Analytics (`Patient History Interface.png`) | 📋 List of Patient Actions (`Appointment Handling Interface.png`) |
| :---: | :---: |
| <img src="Patient History Interface.png" width="100%" alt="Doctor Earnings Dashboard"/> | <img src="Appointment Handling Interface.png" width="100%" alt="Doctor Appointment Tracking"/> |

| 👤 Bio Customization (`Doctor Own Profile Interface.png`) |
| :---: |
| <img src="Doctor Own Profile Interface.png" width="50%" alt="Doctor Profile Management"/> |

### 🛠️ Administrator Panel

| 📈 Global Dashboard (`Admin Dashboard Interface.png`) | 📑 Master Medical Ledger (`History Of All Appointment Interface.png`) |
| :---: | :---: |
| <img src="Admin Dashboard Interface.png" width="100%" alt="Admin Metrics Dashboard"/> | <img src="History Of All Appointment Interface.png" width="100%" alt="All Appointments Ledger"/> |

| 🩺 Specialist Provisioning (`New Doctor Registration Interface.png`) | 👥 Provider Directory (`Docter List Interface.jpg`) |
| :---: | :---: |
| <img src="New Doctor Registration Interface.png" width="100%" alt="Add New Doctor Form"/> | <img src="Docter List Interface.jpg" width="100%" alt="Admin Doctor Management View"/> |

### 🔑 Authentication Gateways

| 🔐 User & Admin Login (`Login Interface.png` & `Admin Login Interface.png`) | 🩺 Doctor Authentication (`Docter Login Interface.png`) |
| :---: | :---: |
| <img src="Login Interface.png" width="100%" alt="User Signup/Login"/> | <img src="Docter Login Interface.png" width="100%" alt="Doctor Specific Security Gateway"/> |

---

## ✨ Features

### 👤 Patient Experience
- **Smart Appointment Scheduling:** Select specialized doctors and pick real-time dynamic date slots and specific hours.
- **Appointment Management:** Cancel unwanted appointments or seamlessly route to payment modules.
- **Integrated Payment Infrastructure:** Mock-ready integration workflows for options like Razorpay.
- **Detailed Personal Profile:** Update contact information, birthday profiles, and generic identifiers.

### 🩺 Doctor Experience
- **Performance Overview Dashboard:** Keep absolute track of total completed consultations, total distinct patients, and localized currency earnings.
- **Instant Status Triggers:** Accept or cancel specific scheduled patient sessions on a per-row context.
- **Professional Bio Builders:** Update specialized credentials (e.g., M.B.B.S., D.O.), consultation fees, experience metrics, and physical clinic locations.

### 🛡️ Administrative Command
- **Platform Analytics:** Real-time summary counts of registered doctors, aggregate appointments, and absolute unique patients.
- **Specialist Onboarding:** Seamlessly fill out customized forms to register authenticated medical practitioners into the data network.
- **Master Registry Access:** View, analyze, and inspect absolute logs across all entries created platform-wide.

---

## 🛠️ Tech Stack

### Frontend
- **Framework:** React.js
- **Styling:** Tailwind CSS (Clean, component-driven layouts)
- **Routing:** React Router DOM

### Backend & Database
- **Runtime Environment:** Node.js
- **Server Framework:** Express.js
- **Database:** MongoDB (using Mongoose ODM)
- **Authentication:** Role-tailored JWT tokens & Bcrypt password hashing

---

## 📂 Project Architecture

```text
Health-Meet/
├── client/                 # Frontend - React.js Core
│   ├── src/
│   │   ├── components/     # Navbars, Sidebars, Route guards
│   │   ├── context/        # State handlers (Admin, Doctor, App context)
│   │   ├── pages/          # Layout blocks (Dashboards, Booking slots, Forms)
│   │   └── App.js          # Core Router mapping
│   └── package.json
│
├── server/                 # Backend - Express & Node.js Engine
│   ├── controllers/        # Logical controllers (Admin, Doctor, Patient controllers)
│   ├── models/             # Schema sets (Doctor, User, Appointment collection structures)
│   ├── routes/             # Exposed REST API endpoint wrappers
│   ├── middleware/         # Auth validation interceptors
│   └── server.js           # Network instantiation endpoint
└── README.md
```

---

 🚀 Getting Started

Follow these steps to spin up Health-Meet on your local machine:

### Prerequisites
- [Node.js](https://nodejs.org/) (v16.x or higher)
- [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) URI or a local running daemon string
  
---

### 1. Clone the Project Stack
```bash
git clone [https://github.com/Subhan-N07/Health-Meet.git](https://github.com/Subhan-N07/Health-Meet.git)
cd Health-Meet
```

### 2. Set Up Environment Keys
Create a `.env` file under the `/server` directory:
```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_signing_key
```

### 3. Initialize Server Dependencies & Boot
```bash
cd server
npm install
npm start
```

### 4. Initialize Client Assets & Run Application
Open a clean secondary terminal window:
```bash
cd client
npm install
npm run dev
```

---

## 🤝 Contributing

Contributions make the developer ecosystem a fantastic space to build, innovate, and master new concepts. 

1. Fork the Repository
2. Branch your custom feature (`git checkout -b feature/CoolEnhancement`)
3. Commit the change profiles (`git commit -m 'Added some cool enhancements'`)
4. Push into your tracking branch (`git push origin feature/CoolEnhancement`)
5. File a public Pull Request

---

## 📝 License

Distributed under the MIT License. See `LICENSE` for more information.

---

⭐ **Found this project interesting or functional?** Drop a star to show some support! Maintained by [Subhan Nanda](https://github.com/Subhan-N07).
