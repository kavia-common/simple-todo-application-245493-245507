# Simple Todo App (React Frontend)

This folder contains the React frontend for the simple todo application. It is built with Create React App and runs as a single-page application in the browser.

## Features

The intended behavior of the todo UI includes a complete basic todo workflow.

### Core todo actions

The app is intended to support adding a todo, marking a todo as completed, and deleting a todo.

### Filtering

The app is intended to support filtering the visible list:

- All
- Active
- Completed

### Persistence (localStorage)

The app is intended to persist the todo list in browser `localStorage`, so that a refresh does not clear your current list.

## Getting started

### Install dependencies

```bash
npm install
```

### Run the app (development)

```bash
npm start
```

Then open:

- http://localhost:3000

If you are running in a hosted development environment, use the environment-provided preview URL for port 3000.

### Run tests

```bash
npm test
```

### Build for production

```bash
npm run build
```

## Environment variables

This project uses Create React App environment variables (must be prefixed with `REACT_APP_`). The `.env` file in this folder defines the following values.

### Variables

- `REACT_APP_API_BASE`: Base URL for API requests (if used by the UI).
- `REACT_APP_BACKEND_URL`: Backend URL (if applicable).
- `REACT_APP_FRONTEND_URL`: Public URL where the frontend is hosted.
- `REACT_APP_WS_URL`: WebSocket URL (if applicable).
- `REACT_APP_NODE_ENV`: Environment name (for example, `development`).
- `REACT_APP_NEXT_TELEMETRY_DISABLED`: Telemetry toggle value.
- `REACT_APP_ENABLE_SOURCE_MAPS`: Whether source maps are enabled.
- `REACT_APP_PORT`: Port the dev server should use (commonly `3000`).
- `REACT_APP_TRUST_PROXY`: Whether to trust proxy headers (environment-specific).
- `REACT_APP_LOG_LEVEL`: Logging verbosity (for example, `info`).
- `REACT_APP_HEALTHCHECK_PATH`: Path used for a health check endpoint (environment-specific).
- `REACT_APP_FEATURE_FLAGS`: Feature flags payload (string value in `.env`, often JSON).
- `REACT_APP_EXPERIMENTS_ENABLED`: Enables or disables experiments.

### Using a different configuration

Edit `.env` and restart the dev server for changes to take effect.

Task completed: Replaced the template frontend README with todo-app-specific documentation, including features, localStorage persistence, filtering, how to run the dev server, and environment variables.
