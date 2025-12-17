# 🤖 MernGPT-Chatbot

## Overview

MernGPT-Chatbot is a full-stack, AI-powered chatbot application built using the MERN stack (MongoDB, Express.js, React.js, Node.js) and the OpenAI API. The project demonstrates how to design a secure, scalable, and customizable conversational AI system suitable for real-world applications.

The architecture cleanly separates frontend and backend responsibilities, making the system easy to maintain, extend, and deploy.

---

## ✨ Features

- **AI-Powered Conversations**  
  Leverages OpenAI GPT models to generate intelligent, context-aware responses.

- **Secure by Design**  
  Implements best practices for handling API keys, cookies, and user data.

- **Scalable Architecture**  
  Built on the MERN stack to support multiple concurrent users and future growth.

- **Highly Customizable**  
  Easily extendable for domain-specific chatbots, assistants, or support systems.

---

## 🛠 Technology Stack

### Frontend
- React.js
- TypeScript
- Vite
- Axios

### Backend
- Node.js
- Express.js
- OpenAI API

### Database
- MongoDB

---

## 🚀 Getting Started

### Prerequisites

Ensure the following are installed on your system:

- Node.js v16 or higher
- MongoDB (running locally or via a cloud provider)
- OpenAI account with an active API key

---

## ⚙️ Installation & Setup

### Backend Setup

1. Navigate to the backend directory:
```bash
cd backend
```

2. Install dependencies:
```bash
npm install
```

3. Configure environment variables:  
   Create a `.env` file inside the backend directory and add:
```env
OPEN_AI_SECRET=your_openai_api_key
OPENAI_ORGANIZATION_ID=your_openai_org_id
COOKIE_SECRET=your_cookie_secret
MONGO_URI=mongodb://localhost:27017/MernGPT
```

⚠️ **Never commit your `.env` file to version control.**

4. Start the backend server:
```bash
npm run dev
```

The backend server will run on port 5000 by default.

---

### Frontend Setup

1. Navigate to the frontend directory:
```bash
cd frontend
```

2. Install dependencies:
```bash
npm install
```

3. Configure API base URL:  
   Update the following line in `frontend/src/main.tsx`:
```typescript
axios.defaults.baseURL = "http://localhost:5000/api/v1";
```

4. Start the frontend development server:
```bash
npm run dev
```

The frontend application will be available at http://localhost:5173.

---

## ▶️ Running the Application

- **Frontend**: http://localhost:5173
- **Backend API**: http://localhost:5000/api/v1

Ensure MongoDB is running before starting the application.

---

## 🏗 Project Structure
```
MernGPT-Chatbot/
├── backend/        # Express server, OpenAI integration, APIs
├── frontend/       # React + TypeScript UI
└── README.md
```

---

## 🙏 Acknowledgements

- [OpenAI](https://openai.com/) — for providing powerful GPT models and APIs

---
