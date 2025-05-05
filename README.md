# 🚀 CodeCrafter – Full-Stack Project Marketplace Platform

**CodeCrafter** is a modern, feature-rich full-stack marketplace platform where users can **buy ready-made projects**, or **place custom project orders** based on their requirements. Built with a sleek and modern UI enhanced by smooth animations, CodeCrafter offers a seamless user experience for both buyers and administrators.

---

## 🌟 Highlights

- 🧑‍💻 Modern UI with **beautiful animations** (Framer Motion, Tailwind CSS)
- 🔐 Secure authentication with **JWT & bcrypt**
- 📦 Ready-made project listing and **custom order placing**
- 🧾 Fully working **transaction system with payment method tracking**
- ⭐ **Review system** for each project
- 👤 **User Dashboard** to manage profile, order history, and transactions
- 🛠️ **Admin Panel** to manage users, projects, orders, and reports
- 📚 Built with clean folder structure and scalable backend architecture

---

## 📌 Core Features

### ✅ User Features

- **Authentication & Authorization**
  - Signup/Login with encrypted password (bcrypt)
  - Token-based session management using JWT

- **Project Marketplace**
  - Browse categorized projects (Web Dev, Full Stack, App Dev, etc.)
  - View detailed project info, price, description, and reviews
  - Purchase with instant confirmation and order tracking
  - Add reviews for purchased projects

- **Custom Project Ordering**
  - If user needs a specific project, they can **place a custom request**
  - Admin/Developer can later fulfill the request and update the download link

- **User Dashboard**
  - View & update profile (username, bio, phone)
  - See all past orders and transactions
  - Manage reviews and placed custom orders

### 🔧 Admin Features

- **Dashboard Panel**
  - View all users, block/unblock users
  - Manage project listings (add/edit/delete)
  - Handle custom orders from users
  - Monitor all transactions and payment statuses
  - Respond to flagged issues or failed payments

---

## 💻 Tech Stack

| Layer       | Tech Used                          |
|-------------|------------------------------------|
| Frontend    | React.js, Axios, Tailwind CSS, Framer Motion |
| Backend     | Node.js, Express.js                |
| Database    | MongoDB + Mongoose ODM             |
| Auth        | bcrypt, JSON Web Token (JWT)       |
| Deployment  | Coming Soon (Render / Vercel)      |

---

## 🧾 Backend Modules

- **Models** – User, Project, Order, Transaction, Review
- **Routes** – Auth, Projects, Orders, Users, Admin, Transactions
- **Controllers** – Cleanly separated logic for modular code
- **Middleware** – Auth guards, role checks, error handling

---

## 📦 Database Design

- `User` ⟶ Has many `Order`, `Review`, `Transaction`
- `Project` ⟶ Has many `Review`
- `Order` ⟶ Belongs to User + Project, has one `Transaction`
- `Transaction` ⟶ Linked with `Order` + `User`

---

## 🧑‍💻 How to Run Locally

```bash
# Clone Repository
git clone https://github.com/your-username/codecrafter.git
cd codecrafter

# Install dependencies
npm install

# Create a .env file and add the following:
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret

# Start Server
npm run dev




---

📝 **Note:** Replace GitHub links and environment variables with your actual values. 

