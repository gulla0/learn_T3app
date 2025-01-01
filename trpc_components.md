# Understanding tRPC in a T3 App

In a T3 app, tRPC serves as a bridge between the frontend and backend, enabling seamless and type-safe communication. Here's a breakdown of its components and their roles:

## tRPC Router

This is where you define your API's endpoints, known as procedures. Each procedure can be a query (for fetching data) or a mutation (for modifying data). These routers are typically defined in the `server/api/routers` directory.

## Context

The context provides shared data to all tRPC procedures, such as database connections or authentication information. It's defined in `server/api/trpc.ts` and ensures that procedures have access to necessary resources.

## API Handler

The entry point for your tRPC API is usually set up in `pages/api/trpc/[trpc].ts`. This file exposes the tRPC router and handles incoming API requests. In Next.js, this is achieved using the `createNextApiHandler` function.

## Frontend Integration

On the client side, tRPC integrates with React Query to provide hooks for calling your API procedures. This setup is often configured in `utils/api.ts`, where you create the tRPC client and define how it communicates with the server.