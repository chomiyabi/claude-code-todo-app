# Todo App Project

## Tech Stack
- React Router v7
- SQLite
- Vitest (unit testing)
- Playwright (E2E testing)
- Cloudflare Workers (deployment)

## Commands
- npm run dev: Start development server
- npm run build: Build for production
- npm run test: Run unit tests
- npm run test:e2e: Run E2E tests
- npm run typecheck: Run TypeScript type checking
- npm run lint: Run ESLint
- npm run format: Format code with Prettier
- npm run deploy: Deploy to Cloudflare Workers

## Code Style
- Use TypeScript strict mode
- Use ES modules (import/export), not CommonJS
- Prefer function components with hooks
- Use 2-space indentation
- Destructure imports when possible
- Use named exports for components

## Architecture
- /app/routes: React Router v7 route files
- /app/components: Reusable UI components
- /app/lib: Business logic and utilities
- /app/db: Database schema and queries
- /tests: Test files (Vitest)
- /e2e: End-to-end tests (Playwright)

## Database
- Use SQLite with better-sqlite3
- Migrations in /app/db/migrations
- Use prepared statements for queries
- Handle transactions properly

## Testing
- Write tests for all new features
- Run tests before committing
- Use Testing Library for component tests
- Test database operations with in-memory SQLite

## Deployment
- Environment variables in wrangler.toml
- Use Cloudflare D1 for production database
- Handle CORS properly for API routes
- Use Cloudflare KV for session storage

## Workflow
- Always run typecheck and lint after code changes
- Test locally before deployment
- Use semantic commit messages
- Keep components small and focused
- Document complex logic with comments only when necessary
- Run typecheck and lint after completing tasks and be sure they ALWAYS pass