# 💬 Chatify - Realtime Chat Application

A full-stack real-time chat application built with the **MERN stack** (MongoDB, Express, React, Node.js) and **Socket.io**. This project features secure authentication, real-time messaging, global state management with Zustand, and advanced security features like rate limiting and bot protection.

## 🚀 Features

* **Real-time Messaging:** Instant message delivery using Socket.io.
* **Authentication:** Secure Signup/Login with JWT (JSON Web Tokens).
* **Online Status:** See who is online in real-time.
* **Image Support:** Upload and send images in chat using Cloudinary.
* **Security:** Rate limiting and bot protection using **Arcjet**.
* **Email Notifications:** Welcome emails sent via **Resend**.
* **Modern UI:** Built with **Tailwind CSS** and **DaisyUI** for a sleek, responsive design.
* **Global State:** Managed efficiently with **Zustand**.
* **Error Handling:** Robust error handling on both client and server.

## 🛠️ Tech Stack

### **Backend**
* **Node.js & Express:** API Server.
* **MongoDB:** Database for users and messages.
* **Socket.io:** Real-time bidirectional event-based communication.
* **Arcjet:** Security shield (Rate limiting & Bot protection).
* **Resend:** Email API service.
* **Cloudinary:** Cloud storage for images.
* **Cookie Parser:** For parsing secure HTTP-only cookies.

### **Frontend**
* **React:** UI Library.
* **Vite:** Fast build tool.
* **Tailwind CSS:** Utility-first CSS framework.
* **DaisyUI:** Component library for Tailwind.
* **Zustand:** State management.
* **Axios:** HTTP client.
* **React Hot Toast:** Notifications.

---

## ⚙️ Environment Variables

To run this project, you will need to add the following environment variables to your `.env` file in the **backend** folder.

`backend/.env`

```env
# Server Configuration
PORT=3000
NODE_ENV=development

# Database
MONGO_URI=your_mongodb_connection_string

# Security (JWT)
JWT_SECRET=your_super_secret_key

# Cloudinary (Image Uploads)
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret

# Frontend URL (CORS)
CLIENT_URL=http://localhost:5173

# Resend (Email Service)
RESEND_API_KEY=your_resend_api_key
EMAIL_FROM=onboarding@resend.dev
EMAIL_FROM_NAME=Chatify

# Arcjet (Rate Limiting)
ARCJET_KEY=your_arcjet_key
ARCJET_ENV=development
