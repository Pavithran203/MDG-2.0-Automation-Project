# MDG 2.0 Automation Project

Playwright and TypeScript end-to-end automation for MDG 2.0 login roles and workflows.

## Current example: role login smoke test

The included suite covers login checks for the **Initiator, Validator, Reviewer, Cataloguer, and QC** roles. After configuring authorized test credentials locally, install dependencies and browsers, then run:

    npm install
    npx playwright install
    npm test

Use the individual scenario-NN npm scripts when you need to run a single included scenario. Consult package.json for the available script names.

**Scope note:** role login automation and helper tooling are included. Business workflows such as creating a request, validation, review, cataloguing, and QC are not implemented yet.

## Included
- src/: Playwright page objects, role configuration, and results reporter.
- tests/: included login and MDG 2.0 scenarios.
- package.json, lockfile, Playwright/TypeScript configuration, and .env.example.
- Full source tree: project-source.zip at the repository root. Download and extract it before setup.

Requires Node.js 18 or newer. Copy .env.example to .env and add only credentials you are authorized to use. Real credentials, generated reports, browser artifacts, and dependencies are excluded; never commit .env.
