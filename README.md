# PNB SRMS

Service Request Management System (PNB SRMS) is a monorepo built with Turborepo.

## Tech Stack

- **Frontend**: [Vite](https://vitejs.dev/) + [React](https://react.dev/) + [TypeScript](https://www.typescriptlang.org/) + [Tailwind CSS](https://tailwindcss.com/)
- **Backend**: [Express](https://expressjs.com/) + [TypeScript](https://www.typescriptlang.org/)
- **Database**: [Neon](https://neon.tech/) (PostgreSQL) + [Prisma](https://www.prisma.io/)
- **Authentication**: [BetterAuth](https://better-auth.com/)
- **Monorepo Tools**: [Turborepo](https://turbo.build/)

## Workspace Structure

### Apps

- `apps/web`: The frontend application.
- `apps/api`: The backend API.

### Packages

- `packages/db`: Shared Prisma client and database schema.
- `packages/types`: Shared TypeScript interfaces and types.
- `packages/ui`: Shared UI components (Shadcn-ready).
- `packages/eslint-config`: Shared ESLint configurations.
- `packages/typescript-config`: Shared TypeScript configurations.

## Getting Started

### Prerequisites

- Node.js (v18+)
- npm (v10+)

### Installation

1.  Install dependencies:

    ```bash
    npm install
    ```

2.  Set up environment variables:
    - Create a `.env` file in `packages/db` (or root) with `DATABASE_URL`.
    - Create `.env` files in `apps/api` and `apps/web` as needed.

### Development

To start the development server for all apps:

```bash
npx turbo dev
```

### Build

To build all apps and packages:

```bash
npx turbo build
```

### Lint

To lint all apps and packages:

```bash
npx turbo lint
```
