# MDG 2.0 Automation

> Full source tree is included in `project-source.zip` at the repository root. Unpack it to restore the directories and files summarized below.

Playwright and TypeScript end-to-end automation for MDG 2.0 login roles and workflow scenarios.

## Included files

- `src/`: Playwright page objects, role configuration, and results reporter.
- `tests/`: scenario tests for login, dashboards, and MDG 2.0 library workflows.
- `package.json`, `package-lock.json`, `playwright.config.ts`, `tsconfig.json`, and `.env.example`: dependencies and local configuration template.

The real `.env`, login report, generated browser artifacts, and dependencies are excluded.

## Run locally

Requires Node.js 18 or newer. Unpack `project-source.zip`, then run `npm install` and `npx playwright install`. Copy `.env.example` to `.env` and enter credentials you are authorized to use. Run `npm test` for the suite or use a `scenario-NN` npm script for one scenario.
