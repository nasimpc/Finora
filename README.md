# 💰 Finora

**Finora** is a Node.js and Express.js web application that helps users **track and manage their expenses** efficiently.  
It includes features like authentication, premium membership, AWS S3 integration for downloads, and both SQL/NoSQL database support.

---

## 🚀 Features

- 🧾 **User Authentication & Authorization**
  - Signup and Signin functionality.
  - Password encryption using **bcrypt**.
  - JWT-based authentication for secure session management.
  - Forgot password functionality via **Sendinblue** email integration.

- 💎 **Premium User Features**
  - Integrated **Razorpay** for upgrading to premium accounts.
  - Premium users can:
    - Download expense reports.
    - View download history.
    - Access a global **leaderboard**.
  - Custom UI enhancements for premium users.

- 💰 **Expense Management**
  - Track expenses, income, and savings.
  - Real-time analytics displayed on the frontend.

- ☁️ **AWS S3 Integration**
  - Securely stores and retrieves user expense data for downloads.

- 🗃️ **Database**
  - Implemented using both **Sequelize (MySQL)** and **Mongoose (NoSQL)** for flexibility and scalability.

---

## 🧑‍💻 Tech Stack

| Category | Technologies |
|-----------|---------------|
| **Frontend** | HTML, CSS, JavaScript |
| **Backend** | Node.js, Express.js |
| **Database** | MySQL (Sequelize ORM), MongoDB (Mongoose) |
| **Authentication** | JWT, bcrypt |
| **Email Service** | Sendinblue (SIB) |
| **Payment Integration** | Razorpay |
| **Cloud Storage** | AWS S3 |

---


