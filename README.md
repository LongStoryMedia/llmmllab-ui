# llmmllab-ui

React-based user interface for interacting with the llmmllab API services.

## Features

- Modern React implementation using TypeScript and Vite
- Material UI Joy interface components
- Real-time streaming responses for chat and completions
- Document upload and processing
- Multi-modal capabilities (text and image generation)
- Responsive design for desktop and mobile

## Tech Stack

- React 19 with TypeScript
- Vite build system
- Material UI Joy
- ESLint with TypeScript configuration
- Playwright for e2e tests

## Getting Started

### Prerequisites

- Node.js 18+
- npm

### Installation

```bash
# Install dependencies
npm install
```

### Development

```bash
# Run development server
npm run dev
```

### Building for Production

```bash
# Build for production
npm run build
```

### Testing

```bash
# Run unit tests
npm run test

# Run e2e tests
npm run test:e2e

# Run e2e tests with UI
npm run test:e2e:ui
```

### Linting

```bash
# Run ESLint
npm run lint
```

## Deployment

The UI can be deployed using the included deployment script:

```bash
./deploy.sh
```

This will build the project and deploy it to the production server.

## Environment Configuration

The project includes multiple environment configuration files:

- `.env.dev` - Development environment settings
- `.env.prod` - Production environment settings
- `.env.local` - Local overrides (not committed to version control)

## Integration with Backend Services

This UI connects to the llmmllab services:

- **llmmllab-server** - REST API server (FastAPI)
- **llmmllab-composer** - gRPC service for workflow orchestration
- **llmmllab-runner** - gRPC service for model execution

API endpoints are configured in the environment files.

## Project Structure

```
ui/
├── src/
│   ├── main.tsx              # Entry point
│   ├── Router.tsx            # React Router configuration
│   ├── components/           # Reusable components
│   ├── pages/                # Page components
│   ├── hooks/                # Custom React hooks
│   ├── lib/                  # Utility libraries
│   └── types/                # TypeScript type definitions
├── e2e/                      # End-to-end tests
├── test/                     # Unit tests
├── public/                   # Static assets
├── components.json           # Component configuration
├── vite.config.ts            # Vite configuration
└── tsconfig.json             # TypeScript configuration
```

## Dependencies

- **llmmllab-server** - REST API server
- **llmmllab-composer** - gRPC service for workflow orchestration
- **llmmllab-runner** - gRPC service for model execution