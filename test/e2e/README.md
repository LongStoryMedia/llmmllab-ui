# UI End-to-End Tests

This directory contains Playwright end-to-end tests for the UI component.

## Running Tests

```bash
cd ui
npm run test:e2e
```

## Test Structure

```
ui/test/e2e/
├── __init__.py          # Python package marker
├── spec/                # TypeScript test specs (optional)
└── README.md            # This file
```

## Playwright Configuration

See `ui/playwright.config.ts` for test configuration.

## E2E Test Directory

This directory is for Playwright e2e tests written in TypeScript.
Tests can be added in the `spec/` subdirectory.