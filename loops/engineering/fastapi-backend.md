# FastAPI backend

> Stand up a real backend with auth, CRUD, a database, and tests, not a toy script.

## Goal (the what)

- **Objective:** Build a FastAPI backend.
- **Success criteria:** JWT user authentication, CRUD endpoints for tasks, PostgreSQL integration, proper error handling, and passing tests.
- **Constraints:** Use standard FastAPI patterns. No secrets in code. Migrations, not manual schema edits.
- **Context:** The data model for tasks and users, and the target Python/Postgres versions.

## Loop (the how)

- **Think:** Decide the next slice to build (models, auth, an endpoint, a test).
- **Act:** Write the code or the test.
- **Observe:** Run the test suite and the app, read the results.
- **Reflect / Plan:** Fix failures, pick the next slice.
- **Stop when:** Auth, CRUD, and Postgres all work, error handling is in place, and the test suite passes.

## Starter prompt

```
Build a FastAPI backend with: JWT user authentication, CRUD endpoints for tasks,
PostgreSQL integration via migrations, and proper error handling. Write tests for the
auth flow and each endpoint. Build it in slices, running the suite after each. Keep
secrets out of code. Stop only when auth, CRUD, and Postgres all work and the full
test suite passes. Show the final test output.
```
