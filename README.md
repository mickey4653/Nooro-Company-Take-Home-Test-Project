# Todo App - Full Stack Application

A modern, responsive Todo application built with Next.js frontend and Express.js backend.

## 🚀 Live Demo

- **Frontend**: [[Your Frontend URL]](https://github.com/mickey4653/todo-list-app-frontend)
- **Backend API**: [[Your Backend URL]](https://github.com/mickey4653/todo-list-app-backend)

## 📋 Project Overview

This is a full-stack Todo application built for a job interview assessment. It demonstrates modern web development practices with a focus on clean code, type safety, and user experience.

### Features

- ✨ **Beautiful UI**: Modern dark theme with gradient accents
- 📱 **Responsive Design**: Works perfectly on all devices
- ⚡ **Real-time Updates**: Optimistic UI updates for better UX
- 🔒 **Type Safety**: Full TypeScript implementation
- 🎨 **Custom Design System**: Consistent styling with Tailwind CSS
- 🗄️ **Database Integration**: MySQL with Prisma ORM
- 🔄 **REST API**: Clean, documented API endpoints

## 🏗️ Architecture

```
┌─────────────────┐    HTTP/JSON    ┌─────────────────┐
│   Next.js       │ ◄─────────────► │   Express.js    │
│   Frontend      │                 │   Backend       │
│                 │                 │                 │
│ • React         │                 │ • REST API      │
│ • TypeScript    │                 │ • Prisma ORM    │
│ • Tailwind CSS  │                 │ • MySQL         │
│ • App Router    │                 │ • Validation    │
└─────────────────┘                 └─────────────────┘
```

## 🛠️ Tech Stack

### Frontend
- **Framework**: Next.js 15 (App Router)
- **Language**: TypeScript
- **Styling**: Tailwind CSS
- **State Management**: React Hooks
- **Icons**: Custom SVG icons

### Backend
- **Runtime**: Node.js
- **Framework**: Express.js
- **Language**: TypeScript
- **Database**: MySQL 8.0
- **ORM**: Prisma
- **Validation**: Zod
- **Containerization**: Docker

## 📁 Repository Structure

This project consists of two separate repositories:

### 1. Frontend Repository
- **Location**: `frontend/`
- **Repository**: [Your Frontend Repo URL]
- **Tech**: Next.js, TypeScript, Tailwind CSS

### 2. Backend Repository
- **Location**: `backend/`
- **Repository**: [Your Backend Repo URL]
- **Tech**: Express.js, Prisma, MySQL

## 🚀 Quick Start

### Prerequisites
- Node.js 18+
- Docker & Docker Compose
- Git

### 1. Clone Both Repositories
```bash
# Frontend
git clone <frontend-repo-url>
cd todo-app-frontend

# Backend (in another terminal)
git clone <backend-repo-url>
cd todo-app-backend
```

### 2. Start Backend
```bash
cd backend
npm install
docker compose up -d
cp env.example .env
npx prisma generate
npx prisma db push
npm run dev
```

### 3. Start Frontend
```bash
cd frontend
npm install
cp env.local.example .env.local
npm run dev
```

### 4. Open Application
- Frontend: http://localhost:3000
- Backend API: http://localhost:4000

## 📖 API Documentation

### Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/health` | API health check |
| `GET` | `/tasks` | Get all tasks |
| `POST` | `/tasks` | Create new task |
| `PUT` | `/tasks/:id` | Update task |
| `DELETE` | `/tasks/:id` | Delete task |

### Request/Response Examples

**Create Task**
```bash
curl -X POST http://localhost:4000/tasks \
  -H "Content-Type: application/json" \
  -d '{"title":"Buy groceries","color":"blue"}'
```

**Get All Tasks**
```bash
curl http://localhost:4000/tasks
```

## 🎨 Design System

The application uses a custom design system built with Tailwind CSS:

- **Colors**: 8 predefined colors (red, orange, yellow, green, blue, purple, pink, brown)
- **Typography**: Consistent font weights and sizes
- **Spacing**: Systematic spacing scale
- **Layout**: Mobile-first responsive design

## 🔧 Development

### Running Tests
```bash
# Frontend
cd frontend
npm run lint

# Backend
cd backend
npm run lint
```

### Database Management
```bash
# Generate Prisma client
npx prisma generate

# Push schema changes
npx prisma db push

# View database
npx prisma studio
```

### Docker Commands
```bash
# Start database
docker compose up -d

# Stop database
docker compose down

# Reset database
docker compose down -v && docker compose up -d
```

## 📱 Responsive Design

The application is fully responsive with breakpoints:
- **Mobile**: < 640px
- **Tablet**: 640px - 1024px
- **Desktop**: > 1024px

## 🚀 Deployment

### Frontend Deployment
- **Vercel** (recommended for Next.js)
- **Netlify**
- **AWS Amplify**

### Backend Deployment
- **Railway**
- **Render**
- **Heroku**
- **AWS EC2**

## 🤝 Contributing

This is a job interview assessment project. For learning purposes:

1. Fork the repositories
2. Create feature branches
3. Make improvements
4. Submit pull requests

## 📄 License

This project is part of a job interview assessment.

## 🙏 Acknowledgments

- **Next.js** team for the amazing framework
- **Tailwind CSS** for the utility-first CSS framework
- **Prisma** for the excellent ORM
- **Figma** for the design inspiration

---

**Built with ❤️ for the job interview assessment**
