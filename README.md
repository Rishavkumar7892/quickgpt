# 🤖 QuickGPT - AI Chat and Image Generator

QuickGPT is a full-stack platform that allows users to interact with AI and bring their ideas to life through image generation. It leverages Google Gemini for responses and ImageKit.io for visuals. The system operates on a credit-based model with subscription management through Stripe. Core features include JWT-based authentication, MongoDB integration, and a responsive React + TailwindCSS UI—making QuickGPT secure, scalable, and user-friendly.

## ✨ Key Features

- 🔐 **Secure authentication with JWT and password hashing using bcryptjs**
- 🔒 **Middleware-protected API routes for safe user access**
- 💬 **AI text responses powered by Google Gemini**
- 🎨 **AI-generated images using ImageKit.io**
- 🌍 **Option to publish images for community sharing**
- 📂 **Full chat management: create, view and delete**
- 👤 **User Dashboard – View your own generated content**
- 💵 **Flexible subscription plans via Stripe (Basic, Pro, Premium)**
- ⚡ **Modern UI with React + Vite + TailwindCSS**
- 🚀 **Deployed on Vercel**

## 🛠️ Tech Stack

### Frontend:
- **React.js**
- **Tailwind CSS**
- **react-hot-toast**
- **Axios**
- **PrismJS**
- **react-markdown**

### Backend:
- **Node.js**
- **Express.js**
- **MongoDB**
- **JWT**
- **bcryptjs**
- **Svix**
- **CORS**
- **Stripe**

### AI Services
- **Google Gemini (text)**
- **ImageKit.io (images)**

---

## Getting Started

### Prerequisites

- Node.js
- MongoDB Atlas
- Google Gemini API
- ImageKit
- Stripe

### 📦 Installation

1. **Clone the repository**

```bash
git clone https://github.com/Rishavkumar7892/quickgpt
cd quickgpt
```

2. **Install client dependencies**

```bash
cd client
npm install
```

3. **Install server dependencies**

```bash
cd server
npm install
```

4. **Create `.env` file in `server` directory**

```env
JWT_SECRET= your_jwt_secret
MONGODB_URI= your_mongodb_connection_string
GEMINI_API_KEY= your_gemini_api_key
IMAGEKIT_PUBLIC_KEY= your_imagekit_public_key
IMAGEKIT_PRIVATE_KEY= your_imagekit_private_key
IMAGEKIT_URL_ENDPOINT= your_imagekit_url
STRIPE_PUBLISHABLE_KEY= your_stripe_publishable_key
STRIPE_SECRET_KEY= your_stripe_secret
STRIPE_WEBHOOK_SECRET= your_webhook_secret
```
5. **Create `.env` file in `client` directory**

```env
VITE_BACKEND_URL=http://localhost:3000
```

6. **Run the application**

```bash
# Start client
cd client
npm run dev

# Start server
cd server
npm run server
```