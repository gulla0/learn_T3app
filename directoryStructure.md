
## Directory Details

- **`prisma/`**: Contains Prisma schema for defining database models.
  - **`schema.prisma`**: File to define your database models.

- **`public/`**: Static files like images and icons.

- **`src/`**: Main source code for the application.
  - **`pages/`**: Next.js Pages Router.
    - **`api/`**: API routes for server-side logic.
      - **`trpc/`**: tRPC handler for backend communication.
    - **`index.tsx`**: Homepage of the app.
  - **`server/`**: Backend logic for the app.
    - **`api/routers/`**: Contains tRPC routers to manage backend procedures.
    - **`context.ts`**: Shared context for tRPC (e.g., database connections).
  - **`styles/`**: Global CSS setup, often used for Tailwind CSS.
  - **`utils/`**: Utility files such as the tRPC client setup.

- **`.env`**: Stores environment variables like database connection strings.

