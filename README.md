# TaskFlow — Auth-Enabled Task Manager with AI Chat

> A full-stack task management app with user authentication and an integrated AI chat assistant.

![Next.js](https://img.shields.io/badge/Next.js-16-black?logo=next.js&logoColor=white)
![React](https://img.shields.io/badge/React-19-blue?logo=react&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-5-blue?logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3-38B2AC?logo=tailwind-css&logoColor=white)
![better-auth](https://img.shields.io/badge/Auth-better--auth-purple)
![React Query](https://img.shields.io/badge/React_Query-5-red?logo=reactquery&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)

## Overview

TaskFlow is a productivity app that combines task management with an AI chat assistant. Users can register, log in, create/edit/delete tasks, and interact with an AI chat panel — all within a single, responsive Next.js application.

## Features

- **User Authentication** — Register and login with `better-auth`
- **Protected Routes** — Auth-gated task management pages
- **Task CRUD** — Create, edit, and delete tasks with a clean modal interface
- **AI Chat Panel** — Integrated chat UI with message history
- **Type-Safe** — Full TypeScript coverage with strict type checking
- **Formatted Code** — Prettier + ESLint configured out of the box

## Tech Stack

| Technology | Role |
|---|---|
| Next.js 16 | Full-stack framework (App Router) |
| React 19 | UI library |
| TypeScript 5 | Type safety |
| better-auth | Authentication library |
| TanStack React Query 5 | Server state & data fetching |
| Tailwind CSS 3 | Styling |
| Prettier | Code formatting |
| ESLint | Linting |

## Getting Started

```bash
# Clone
git clone https://github.com/SyedShahmeerAH/copy.git
cd copy

# Install dependencies
npm install

# Start dev server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000).

## Project Structure

```
src/
  app/
    login/           # Login page
    register/        # Registration page
    tasks/           # Protected task management page
    layout.tsx       # Root layout with providers
    page.tsx         # Landing/home page
    providers.tsx    # App-wide providers (React Query, auth)
    globals.css      # Global styles + Tailwind
  components/
    Header.tsx       # Navigation header
    ProtectedRoute.tsx  # Auth guard wrapper
    AddTaskForm.tsx  # Task creation form
    TaskItem.tsx     # Individual task display
    EditTaskModal.tsx  # Task edit modal
    ChatPanel.tsx    # AI chat container
    ChatInput.tsx    # Chat message input
    ChatMessage.tsx  # Individual chat message
  lib/               # Utilities and API helpers
  types/             # TypeScript type definitions
```

## Scripts

| Command | Description |
|---|---|
| `npm run dev` | Start development server |
| `npm run build` | Production build |
| `npm run start` | Start production server |
| `npm run lint` | Run ESLint |
| `npm run format` | Format code with Prettier |
| `npm run type-check` | TypeScript type checking (no emit) |

## License

MIT