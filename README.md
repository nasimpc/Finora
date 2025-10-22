# Finora

---

**Finora** is a full-featured web-based expense tracking application that helps users efficiently manage their income, expenses, and savings.  
It supports secure authentication, premium memberships, real-time analytics, and AWS-integrated download functionality.  

The platform have implemented first in **MySQL (Sequelize)** and then in **MongoDB (Mongoose)** and is deployed on **AWS**.

---

## Features

- **User Authentication & Authorization**
  - Signup and Signin functionality.
  - Password encryption using **bcrypt**.
  - JWT-based authorization for secure access.
  - Forgot password functionality via **Sendinblue** email service.

- **Premium User Features**
  - Integrated **Razorpay** for upgrading to premium accounts.
  - Premium users can:
    - Download their expense reports.
    - View download history.
    - Access a global **leaderboard**.
  - Exclusive UI elements and themes for premium users.

- **Expense Management**
  - Track daily expenses, credits, and savings.
  - Dynamic dashboard showing financial summaries and analytics.

- **AWS Integration**
  - Download functionality implemented via **AWS S3** for secure file storage.

- **Database**
  - Dual database support:
    - **MySQL** with **Sequelize ORM** for structured data.
    - **MongoDB** with **Mongoose** for flexible document storage.

---

## Tech Stack

| Category | Technologies |
|----------|--------------|
| **Frontend** | HTML, CSS, JavaScript |
| **Backend** | Node.js, Express.js |
| **Databases** | MySQL (Sequelize ORM), MongoDB (Mongoose) |
| **Authentication** | JWT, bcrypt |
| **Email Service** | Sendinblue (SIB) |
| **Payment Integration** | Razorpay |
| **Cloud Storage** | AWS S3 |

---

## Getting Started

### 1️⃣ Clone the repository
```bash
git clone https://github.com/yourusername/finer.git
cd finer
````

### 2️⃣ Install dependencies

```bash
npm install
```

### 3️⃣ Create a `.env` file

Example configuration:

```env
PORT='3000'
JWT_SECRET_KEY='secretkey'

# Sendinblue API Key
SIB_API_KEY='xxxxxxxxxxxxxxxxxxxxxxxx'

# Razorpay Keys
RAZORPAY_KEY_ID='xxxxxxxxxxxx'
RAZORPAY_SECRET='xxxxxxxxxxxx'

# AWS Keys
BUCKET_NAME='your-bucket'
AWS_ACCESS_KEY_ID='xxxxxxxxxxxx'
AWS_SECRET_ACCESS_KEY='xxxxxxxxxxxx'

# Database Configurations
MYSQL_DB_NAME='finer'
MYSQL_USERNAME='root'
MYSQL_PASSWORD='password'
MYSQL_DIALECT='mysql'
MYSQL_HOST='localhost'

MONGODB_URI='mongodb://localhost:27017/finer'
```

### 4️⃣ Start the application

```bash
npm start
```

### 5️⃣ Access the app

Visit:

```
http://localhost:3000
```

---


---

## 🧠 Architecture Highlights

* **Secure Authentication:** JWT and bcrypt.
* **Cloud Integration:** AWS S3 for file management.
* **Payment Gateway:** Razorpay for premium purchases.
* **Email Automation:** Sendinblue for password recovery.
* **Hybrid Database Model:** Combines relational and NoSQL data management.

---

---

Would you like me to make an additional **short version (for portfolio)** that summarizes Finer in 4–5 lines for display on your GitHub profile or personal site?
```
