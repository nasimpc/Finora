
---

# Finora

A full-stack **Node.js/Express.js** web application, here users can register, log in, manage their finances, and even unlock **premium features** like data downloads, leaderboards, and expense history tracking.

---

## **Features**

* **Expense Management:** Add, view, and delete expenses easily.
* **User Authentication & Authorization:** Secure sign-in using **bcrypt** for password encryption and **JWT** for user sessions.
* **Password Reset:** Forgot password feature implemented via **SendinBlue (SIB)** for email recovery.
* **Premium Membership:** Integrated **Razorpay** payment gateway to upgrade users to premium accounts.
* **Cloud Integration:** Download and backup expense reports using **AWS S3**.
* **Premium Dashboard:** Includes a **leaderboard**, **expense download history**, and **advanced UI** for premium users.
* **Hybrid Database:** Integrated both **MySQL (Sequelize ORM)** and **MongoDB (Mongoose)** for data management and flexibility.

---

## **Tech Stack**

**Frontend:** HTML, CSS, JavaScript
**Backend:** Node.js, Express.js
**Database:** MySQL (Sequelize), MongoDB (Mongoose)
**Cloud & Security:** AWS S3, JWT, Bcrypt, SendinBlue, Razorpay

---

## **Installation & Setup**

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/finer-expense-tracker.git
   cd finer-expense-tracker
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Create a `.env` file in the root directory and configure it as follows:

   ```env
   PORT='3000'
   JWT_SECRET_KEY='secretkey'
   SIB_API_KEY='your-sendinblue-api-key'
   RAZORPAY_KEY_ID=''
   RAZORPAY_KEY_SECRET=''

   WEBSITE="http://localhost:3000"

   BUCKET_NAME='your-aws-bucket'
   AWS_ACCESS_KEY_ID='your-aws-key'
   AWS_SECRET_ACCESS_KEY='your-aws-secret'

   DATABASE_NAME='expense-tracker'
   DATABASE_USERNAME='root'
   DATABASE_PASSWORD='yourpassword'
   DATABASE_DIALECT='mysql'
   DATABASE_HOST='localhost'
   ```

4. Start the application:

   ```bash
   npm start
   ```

5. Open in your browser:

   ```
   http://localhost:3000
   ```

---

## **API Documentation**

### **Expense Routes**

| Method | Endpoint                      | Description               |
| ------ | ----------------------------- | ------------------------- |
| POST   | `/expense/add-expense`        | Add a new expense         |
| GET    | `/expense/get-expenses`       | Retrieve all expenses     |
| DELETE | `/expense/delete-expense/:id` | Delete a specific expense |

### **Premium Routes**

| Method | Endpoint                    | Description                     |
| ------ | --------------------------- | ------------------------------- |
| POST   | `/premium/leaderboard-data` | Get top users sorted by expense |
| GET    | `/premium/download`         | Download user expense details   |

### **Purchase Routes**

| Method | Endpoint                       | Description                  |
| ------ | ------------------------------ | ---------------------------- |
| POST   | `/purchase/premium-membership` | Upgrade to a premium account |

### **User Routes**

| Method | Endpoint          | Description                        |
| ------ | ----------------- | ---------------------------------- |
| POST   | `/user/add-user`  | Sign up a new user                 |
| POST   | `/user/login`     | Log in existing user               |
| GET    | `/user/get-users` | Fetch all registered users         |
| GET    | `/user/get-user`  | Fetch current user using JWT token |

### **Password Routes**

| Method | Endpoint                    | Description                    |
| ------ | --------------------------- | ------------------------------ |
| POST   | `/password/forget-password` | Send password reset link       |
| GET    | `/password/reset/:id`       | Access password reset form     |
| POST   | `/password/reset`           | Submit and update new password |

---
