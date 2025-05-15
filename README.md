# password-reset
# Password Reset App — Backend

This is the backend for a secure Password Reset application using **Node.js**, **Express**, **MongoDB**, and **JWT**. It allows users to register, login, request password reset via email, and securely update their password using a token.

---

## 🔗 Live URLs

- **Frontend (React)**: [https://your-frontend-url.netlify.app](https://your-frontend-url.netlify.app)
- **Backend (Node + Express)**: [https://your-backend-url.onrender.com](https://your-backend-url.onrender.com)

---

## ⚙️ Technologies Used

- Node.js
- Express.js
- MongoDB + Mongoose
- Bcrypt.js (for password hashing)
- JWT (for authentication)
- Nodemailer (for email service)
- dotenv (.env environment management)

---

## 📦 API Endpoints

| Method | Route | Description |
|--------|--------------------------------------|------------------------------|
| POST | `/api/auth/register` | Register a new user |
| POST | `/api/auth/login` | Login and get JWT token |
| POST | `/api/auth/forgot-password` | Send password reset link |
| POST | `/api/auth/reset-password/:token` | Reset password with token |

---

## 🧪 Postman Collection

You can test all routes using this Postman collection:  
**[Click here to view the Postman collection](https://documenter.getpostman.com/view/44617620/2sB2qWFPDi)**  
(Replace the link with your exported collection URL)

To import:
1. Open Postman
2. Click **"Import"**
3. Paste the link or upload the exported `.json` file

---

## 🛠️ Environment Variables (.env)

Create a `.env` file in your backend folder and add:

```env
PORT=5000
MONGO_URI=your_mongo_connection_string
JWT_SECRET=your_secret_key
EMAIL_USER=your_email@gmail.com
EMAIL_PASS=your_gmail_app_password
FRONTEND_URL=http://localhost:5173/
