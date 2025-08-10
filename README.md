# 🔐 Next.js Login Authentication

A secure and modern authentication system built with **Next.js**, supporting **user registration**, **login**, and **protected routes**.  
This project demonstrates how to integrate **JWT-based authentication**, **API routes**, and **session management** in a Next.js app.

---

## 🚀 Features

- 📦 **Next.js 14+** (App Router / Pages Router supported)
- 🔑 **JWT-based Authentication**
- 🛡 **Secure Password Hashing** using bcrypt
- 🗄 **MongoDB Database** (via Mongoose)
- 🔐 Protected API routes & pages
- 📱 Fully responsive UI
- 🌐 Environment variable configuration
- ✅ Easy to extend for OAuth (Google, GitHub, etc.)

---


yaml
Copy
Edit

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/nextjs-auth.git
cd nextjs-auth
2️⃣ Install Dependencies
bash
Copy
Edit
npm install
# or
yarn install
3️⃣ Create .env.local File
env
Copy
Edit
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
NEXT_PUBLIC_API_URL=http://localhost:3000
4️⃣ Run the Development Server
bash
Copy
Edit
npm run dev
Visit http://localhost:3000 🚀

🛠 API Endpoints
Method	Endpoint	Description	Auth Required
POST	/api//register	Register new user	❌
POST	/api//login	Login user	❌
GET	/api/user	Get user profile	✅

🔒 Authentication Flow
User Registers → Data stored in MongoDB with hashed password.

User Logs In → JWT is generated and stored in HTTP-only cookie.

Protected Routes → Checked via middleware or API route verification.

Logout → Cookie cleared.
<img width="1140" height="906" alt="Screenshot 2025-08-10 161753" src="https://github.com/user-attachments/assets/ec42083a-e2d4-4c04-9371-f2e1c0e6546b" />


