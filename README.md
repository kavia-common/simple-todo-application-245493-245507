# Simple Todo Application (React)

This repository contains a simple React-based todo application. The UI runs entirely in the browser and is designed to be clean and responsive.

## Features

The application supports the core todo workflow.

### Todo management

You can create and manage a list of todos from the UI. The intended feature set includes adding new todos, marking todos as completed, and deleting todos.

### Filtering

The intended feature set includes basic list filtering so that you can switch between viewing all todos, only active todos, or only completed todos.

### Persistence (browser localStorage)

The intended feature set includes persistence in the browser using `localStorage`, so that your todos remain after a refresh.

## Project structure

The React application lives under:

- `frontend_app/`: Create React App-based frontend

## Running the frontend (local preview)

### Prerequisites

You need a recent Node.js LTS version and npm.

### Install dependencies

From the repository root:

```bash
cd frontend_app
npm install
```

### Start the dev server

```bash
cd frontend_app
npm start
```

By default, Create React App runs at:

- http://localhost:3000

If you are running inside a hosted development environment, use the environment-provided preview URL for port 3000.

## Environment variables

The frontend container (`frontend_app`) includes a `.env` file with the following `REACT_APP_*` variables. Create React App only exposes environment variables to the browser when they are prefixed with `REACT_APP_`.

### Available variables

- `REACT_APP_API_BASE`: Base URL for API requests (if the UI uses HTTP APIs).
- `REACT_APP_BACKEND_URL`: Backend URL (if applicable).
- `REACT_APP_FRONTEND_URL`: Public URL where the frontend is hosted.
- `REACT_APP_WS_URL`: WebSocket URL (if the UI uses websockets).
- `REACT_APP_NODE_ENV`: Environment name (for example, `development`).
- `REACT_APP_NEXT_TELEMETRY_DISABLED`: Telemetry toggle value.
- `REACT_APP_ENABLE_SOURCE_MAPS`: Whether source maps are enabled.
- `REACT_APP_PORT`: Port the dev server should use (commonly `3000`).
- `REACT_APP_TRUST_PROXY`: Whether to trust proxy headers (environment-specific).
- `REACT_APP_LOG_LEVEL`: Logging verbosity (for example, `info`).
- `REACT_APP_HEALTHCHECK_PATH`: Path used for a health check endpoint (environment-specific).
- `REACT_APP_FEATURE_FLAGS`: Feature flags payload (string value in `.env`, often JSON).
- `REACT_APP_EXPERIMENTS_ENABLED`: Enables or disables experiments.

### Notes

If you change `.env` values, restart `npm start` so the dev server picks up the new environment.

## Scripts

From `frontend_app/`:

- `npm start`: Run the development server
- `npm test`: Run tests (Create React App test runner)
- `npm run build`: Build a production bundle

Task completed: Updated the root README with app overview, features (including filtering and localStorage persistence), run instructions for the frontend preview, and a documented environment variables section.
