# Project Structure: `my-t3-app`

my-t3-app/
├── **prisma/**                _# Contains the Prisma schema for database setup_
│   └── **schema.prisma**      _# Define your database models here_
├── **public/**                _# Static files (e.g., images, icons)_
├── **src/**                   _# Main source code for the app_
│   ├── **pages/**             _# Next.js Pages Router - defines routes for your app_
│   │   ├── **api/**           _# API routes_
│   │   │   └── **trpc/**      _# tRPC handler for backend communication_
│   │   └── **index.tsx**      _# Homepage of your app_
│   ├── **server/**            _# Backend logic_
│   │   ├── **api/routers/**   _# tRPC routers for your app's backend_
│   │   └── **context.ts**     _# Shared context for tRPC (e.g., database connections)_
│   ├── **styles/**            _# Global CSS (Tailwind setup is here)_
│   └── **utils/**             _# Utility files like tRPC client setup_
└── **.env**                   _# Environment variables (e.g., database connection)_




