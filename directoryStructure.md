# Project Structure: `my-t3-app`

my-t3-app/
├── prisma/                # Contains the Prisma schema for database setup
│   └── schema.prisma      # Define your database models here
├── public/                # Static files (e.g., images, icons)
├── src/                   # Main source code for the app
│   ├── pages/             # Next.js Pages Router - defines routes for your app
│   │   ├── api/           # API routes
│   │   │   └── trpc/      # tRPC handler for backend communication
│   │   └── index.tsx      # Homepage of your app
│   ├── server/            # Backend logic
│   │   ├── api/routers/   # tRPC routers for your app's backend
│   │   └── context.ts     # Shared context for tRPC (e.g., database connections)
│   ├── styles/            # Global CSS (Tailwind setup is here)
│   └── utils/             # Utility files like tRPC client setup
└── .env                   # Environment variables (e.g., database connection)


