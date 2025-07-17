# 🚀 CodeOps - LeetCode Clone with Video Solutions

A full-stack coding platform similar to LeetCode with video solution uploads and AI chat assistance.

## ✨ Features

- 🔐 **User Authentication** - Login/Signup with JWT
- 📝 **Problem Management** - Create, update, delete coding problems
- 💻 **Code Editor** - Monaco editor with multiple language support
- 🎥 **Video Solutions** - Upload and view solution videos via Cloudinary
- 🤖 **AI Chat** - Get help with problems using Gemini AI
- 📊 **Submission History** - Track your coding progress
- 👨‍💼 **Admin Panel** - Manage problems and videos

## 🛠️ Tech Stack

### Backend
- **Node.js** with Express.js
- **MongoDB** with Mongoose
- **Redis** for caching
- **Cloudinary** for video storage
- **JWT** for authentication
- **Gemini AI** for chat assistance

### Frontend
- **React** with Vite
- **Redux Toolkit** for state management
- **TailwindCSS** + **DaisyUI** for styling
- **Monaco Editor** for code editing
- **React Router** for navigation

## 🚀 Quick Start

### Prerequisites
- Node.js (v16+)
- MongoDB
- Redis
- Cloudinary account

### Installation

1. **Clone the repository**
   ```bash
   git clone <your-repo-url>
   cd codeops-leetcode-clone
   ```

2. **Install all dependencies**
   ```bash
   npm run install:all
   ```

   Or install manually:
   ```bash
   # Root dependencies
   npm install

   # Backend dependencies
   cd backend && npm install

   # Frontend dependencies
   cd ../frontend && npm install
   ```

4. **Environment Setup**
   Create `.env` file in `backend/` directory:
   ```env
   MONGO_URI=mongodb://localhost:27017/codeeditor
   JWT_SECRET=your_jwt_secret
   REDIS_URL=your_redis_url
   CLOUDINARY_CLOUD_NAME=your_cloud_name
   CLOUDINARY_API_KEY=your_api_key
   CLOUDINARY_API_SECRET=your_api_secret
   GEMINI_API_KEY=your_gemini_api_key
   ```

5. **Start the application**
   ```bash
   # Start both backend and frontend concurrently
   npm run dev

   # Or start individually:
   npm run dev:backend  # Backend only (port 3000)
   npm run dev:frontend # Frontend only (port 5174)
   ```

## 📁 Project Structure

```
codeops-leetcode-clone/
├── backend/               # Backend API
│   ├── src/
│   │   ├── controllers/   # Route controllers
│   │   ├── models/        # MongoDB models
│   │   ├── routes/        # API routes
│   │   ├── middleware/    # Auth & validation
│   │   ├── config/        # Database & Redis config
│   │   └── utils/         # Helper functions
│   ├── package.json
│   └── .env
├── frontend/              # React frontend
│   ├── src/
│   │   ├── components/    # React components
│   │   ├── pages/         # Page components
│   │   ├── store/         # Redux store
│   │   └── utils/         # Frontend utilities
│   └── package.json
├── package.json           # Root workspace manager
└── README.md
```

## 🎯 Usage

### For Users
1. **Sign up** and create an account
2. **Browse problems** on the homepage
3. **Solve problems** using the code editor
4. **Submit solutions** and track progress
5. **Watch video solutions** in the Editorial tab
6. **Get AI help** using the ChatAI feature

### For Admins
1. **Access admin panel** from user dropdown
2. **Create problems** with test cases
3. **Upload video solutions** for problems
4. **Manage existing problems** (update/delete)

## 🔧 Available Scripts

### Root (Workspace)
- `npm run dev` - Start both backend and frontend
- `npm run dev:backend` - Start backend only
- `npm run dev:frontend` - Start frontend only
- `npm run install:all` - Install all dependencies
- `npm run build` - Build frontend for production
- `npm run kill-port` - Kill process on port 3000

### Backend (cd backend/)
- `npm run dev` - Start with nodemon
- `npm start` - Start production server
- `npm run clean-start` - Kill port and start

### Frontend (cd frontend/)
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build

## 🚀 GitHub Upload Guide

### **Step 1: Initialize Git Repository**
```bash
git init
git add .
git commit -m "Initial commit: LeetCode clone with video solutions and AI chat"
```

### **Step 2: Create GitHub Repository**
1. Go to [GitHub](https://github.com) and create a new repository
2. Name it `codeops-leetcode-clone` or your preferred name
3. **Don't** initialize with README (we already have one)

### **Step 3: Connect and Push**
```bash
git remote add origin https://github.com/yourusername/your-repo-name.git
git branch -M main
git push -u origin main
```

### **Step 4: Set Up Environment Variables**
- Add your `.env` file to `.gitignore` (already included)
- Document required environment variables in README
- Consider using GitHub Secrets for deployment

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📄 License

This project is licensed under the ISC License.

## 🙏 Acknowledgments

- Monaco Editor for the code editor
- Cloudinary for video hosting
- Google Gemini for AI assistance
- TailwindCSS & DaisyUI for beautiful UI
