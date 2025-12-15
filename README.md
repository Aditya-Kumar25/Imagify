# Imagify

Imagify is a full-stack web application that allows users to generate images from text prompts using AI.  
The application uses a **credit-based system** to manage usage and integrates **Razorpay** for secure credit purchases.

---

## Features

- User authentication with **JWT**
- AI-based **text-to-image generation**
- **Credit-based access control**
- Secure payments using **Razorpay**
- Image **download support**
- Responsive **React** frontend

---

## Tech Stack

### Frontend
- React
- React Router
- Context API
- Axios
- Tailwind CSS

### Backend
- Node.js
- Express
- MongoDB (Mongoose)
- JWT Authentication
- Razorpay Payment Gateway
- ClipDrop AI API

---

## Application Flow

1. Users sign up or log in and receive initial **free credits**
2. Each image generation consumes **one credit**
3. Backend validates user and available credits before calling the AI API
4. Generated images are returned as **Base64** and rendered on the frontend
5. Users can purchase additional credits via **Razorpay**
6. Credits are added only after **backend payment verification**

---

## Payment Flow

1. User selects a credit plan
2. Backend creates a transaction and **Razorpay order**
3. Frontend opens **Razorpay Checkout**
4. Backend verifies the payment
5. Credits are updated after successful verification

---

## Project Structure

```bash
backend/
 ├── controllers
 ├── routes
 ├── models
 ├── middlewares
 └── index.js

frontend/
 ├── components
 ├── pages
 ├── context
 └── App.jsx

 MONGODB_URI=
JWT_SECRET=
RAZORPAY_KEY_ID=
RAZORPAY_KEY_SECRET=
CLIPDROP_API=

VITE_BACKEND_URL=
VITE_RAZORPAY_KEY_ID=


If you want, I can also add:
- Installation & setup steps
- API documentation
- Screenshots section
- Live demo link section

