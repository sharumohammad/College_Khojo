🎓 CollegeKhojo

🔗 Live Project: https://khojo-college.vercel.app/home

📌 Status: Active & Deployed

CollegeKhojo is an educational platform designed to help 12th-grade students preparing for entrance exams like JEE, NEET, CUET, CET, and others.
The platform provides a user-friendly interface, mock tests, and secure authentication, helping students practice and track progress easily.

🚀 Key Features
👤 User Authentication

OTP-based secure login system

Modern signup and login flow

Protected pages for authenticated users

📝 Mock Test System (Basis of learning)

Multiple-choice format (MCQ)

Answer selection with scoring

Final summary screen

Study support through structured content

🏫 College Information (Coming Soon)

Students will be able to explore colleges based on:

Exam type

Rank/score

Stream & location

📱 User-Friendly Experience

Fully responsive design

Fast navigation

Clean and minimal UI for students

🛠️ Tech Stack
Layer	Technology
Frontend	React + Vite
UI Styling	Tailwind CSS
Backend	Node.js, Express.js
Database	MongoDB Atlas
Authentication	JWT + OTP Validation (Email / Phone)
Deployment	Vercel (Frontend), Render/Railway (Backend)
🏗️ Architecture Diagram
         ┌───────────────┐
         │   Frontend     │
         │ (React + Vite) │
         └───────┬────────┘
                 │ HTTPS Requests
                 ▼

                 
        ┌──────────────────────┐
        │     Backend API      │
        │ (Node.js + Express)  │
        └───────────┬──────────┘
                    │ Database Queries
                    ▼

                    
          ┌───────────────────────┐
          │   MongoDB (Atlas)     │
          └───────────────────────┘

📡 API Overview
Endpoint	Method	Description
/api/auth/signup	POST	Create account
/api/auth/send-otp	POST	Send OTP
/api/auth/verify-otp	POST	Validate OTP
/api/tests/list	GET	Fetch available mock tests
/api/tests/submit	POST	Submit answers and generate result
🔧 Local Setup Guide
1️⃣ Clone the Repository
git clone https://github.com/yourusername/collegekhojo.git
cd collegekhojo

2️⃣ Backend Setup
cd server
npm install


Create a .env file:

PORT=5000
MONGO_URI=your_mongodb_connection
JWT_SECRET=your_secret_key
OTP_API_KEY=your_provider_key


Run backend:

npm run dev

3️⃣ Frontend Setup
cd client
npm install


Run client:

npm run dev
