---
title: "express-javascript-template Portfolio Skills"
layout: page
---

This page is a living technical record of skills, tools, and engineering practices demonstrated in the [express-javascript-template](https://github.com/blwatkins/express-javascript-template#readme) project.

## Project Overview

- **Project Type:** Web Application Template / Backend Starter
- **Primary Runtime:** [Node.js](https://nodejs.org/en)
- **Primary Framework:** [Express](https://expressjs.com/)
- **Server Rendering Engine:** [EJS](https://ejs.co/)
- **Primary Implementation Language:** [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

## At a Glance

- **CI runtime coverage:** 3 Node.js versions (`20.x`, `22.x`, `24.x`)
- **Automation workflows:** 2 GitHub Actions workflows (lint/build, security analysis)
- **Dependency automation:** Monthly Dependabot updates for npm and GitHub Actions
- **Documentation approach:** README + source-linked technical evidence

## Skills and Tooling Inventory

- **Programming Languages:** [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript), [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML), [Markdown](https://www.markdownguide.org/), [YAML](https://yaml.org/)
- **Runtime & Frameworks:** [Node.js](https://nodejs.org/en), [Express](https://expressjs.com/)
- **Templating & View Layer:** [EJS](https://ejs.co/)
- **HTTP Security:** [`helmet`](https://helmetjs.github.io/), [`cors`](https://github.com/expressjs/cors), [`express-rate-limit`](https://github.com/express-rate-limit/express-rate-limit)
- **Bundling & Frontend Build:** [webpack](https://webpack.js.org/)
- **Code Quality:** [ESLint](https://eslint.org/)
- **Dependency Management:** [npm](https://www.npmjs.com/), [GitHub Dependabot](https://docs.github.com/en/code-security/tutorials/secure-your-dependencies)
- **Versioning & Platform:** [Git](https://git-scm.com/), [GitHub](https://github.com/)
- **CI/CD:** [GitHub Actions](https://github.com/features/actions), [CodeQL](https://codeql.github.com/)
- **Development Runtime Utilities:** [nodemon](https://nodemon.io/)
- **Environment Management:** [n](https://github.com/tj/n)
- **Development Environments:** [WebStorm](https://www.jetbrains.com/webstorm/), [Visual Studio Code](https://code.visualstudio.com/)

## Capability Record

- Express app composition with centralized middleware setup for security and request handling
- Environment-driven runtime configuration with validation and safe defaults
- Server-side rendering flow using EJS and static asset serving for bundled client code
- Webpack-based client bundle pipeline integrated into server startup/build scripts
- Dual ESLint configurations for client/server concerns with style and security rules
- CI-based lint and build verification across multiple Node.js LTS/current versions
- Monthly automated dependency and GitHub Actions update strategy with grouped updates

## Detailed Technical Notes

### Express app composition and middleware stack

- The server initializes a single Express app and configures HTTP hardening and request handling middleware.
- Security and network controls include `helmet`, CORS policy, JSON payload size limits, and request rate limiting.
- Evidence:
    - [`src/app.mjs`](https://github.com/blwatkins/express-javascript-template/blob/main/src/app.mjs)

### Environment-driven runtime configuration

- Runtime constants are centralized and derived from environment variables with parsing/validation.
- `PORT` falls back to a safe default when unset/invalid; `TRUST_PROXY` and `ALLOWED_ORIGINS` are normalized.
- Evidence:
    - [`src/constants.mjs`](https://github.com/blwatkins/express-javascript-template/blob/main/src/constants.mjs)

### Server startup orchestration

- Entrypoint imports the configured app and starts listening on the resolved port.
- This keeps bootstrapping concerns minimal and separate from app composition.
- Evidence:
    - [`src/main.mjs`](https://github.com/blwatkins/express-javascript-template/blob/main/src/main.mjs)

### Server-rendered page with bundled client asset

- The root route renders an EJS view.
- The view loads a webpack-generated browser bundle from `public/dist`.
- Evidence:
    - [`src/app.mjs`](https://github.com/blwatkins/express-javascript-template/blob/main/src/app.mjs)
    - [`views/index.ejs`](https://github.com/blwatkins/express-javascript-template/blob/main/views/index.ejs)
    - [`webpack.config.mjs`](https://github.com/blwatkins/express-javascript-template/blob/main/webpack.config.mjs)
    - [`src-client/index.mjs`](https://github.com/blwatkins/express-javascript-template/blob/main/src-client/index.mjs)

### Quality validation workflows

- CI executes lint and build checks on `push` and `pull_request` events targeting `main`.
- The build matrix verifies compatibility against `20.x`, `22.x`, and `24.x` Node.js versions.
- Evidence:
    - [`.github/workflows/npm-build.yml`](https://github.com/blwatkins/express-javascript-template/blob/main/.github/workflows/npm-build.yml)
    - [`package.json`](https://github.com/blwatkins/express-javascript-template/blob/main/package.json)

### Security analysis and dependency maintenance workflows

- CodeQL analysis runs on push/PR plus a monthly scheduled scan.
- Dependabot is configured for monthly npm and GitHub Actions updates, including grouped production/development dependency policies.
- Evidence:
    - [`.github/workflows/codeql.yml`](https://github.com/blwatkins/express-javascript-template/blob/main/.github/workflows/codeql.yml)
    - [`.github/dependabot.yml`](https://github.com/blwatkins/express-javascript-template/blob/main/.github/dependabot.yml)

### Linting posture and current testing status

- Separate ESLint flat configs are maintained for server and client contexts, with explicit rule sets for correctness, style, Node compatibility, and security.
- The repository currently does not implement automated tests (`npm test` is a placeholder that exits with error).
- Evidence:
    - [`eslint.config.server.mjs`](https://github.com/blwatkins/express-javascript-template/blob/main/eslint.config.server.mjs)
    - [`eslint.config.client.mjs`](https://github.com/blwatkins/express-javascript-template/blob/main/eslint.config.client.mjs)
    - [`package.json`](https://github.com/blwatkins/express-javascript-template/blob/main/package.json)
