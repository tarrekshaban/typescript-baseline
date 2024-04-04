# typescript-baseline

This is the baseline configuration for typescript projects using Express and Node.

## Commands
| Command          | Script                                     | Description                                                     |
|------------------|------------------------------------------ |-----------------------------------------------------------------|
| dev              |`nodemon`                                      | Runs the application in development mode, watching for changes. |
| build            |`rm -rf dist/* && tsc`                    | Deletes the existing build, then compiles TypeScript code.      |
| clean            |`rimraf dist`                           | Deletes the 'dist' output directory.                            |
| clean:build      |`npm run clean && npm run build`          | Deletes the build directory and then rebuilds the project.      |
| clean:build:serve|`npm run clean && npm run build && npm run serve` | Cleans, builds, and then starts the application server.        |
| clean:build:dev  |`npm run clean && npm run build && npm run dev` | Cleans, builds, and starts the app in development mode.          |
| serve            |`node dist/index.js`                       | Starts the production server using the compiled code.           |
| lint             |`eslint . --ext .ts`                       | Checks TypeScript code for style and potential errors.          |
| lint:fix         |`eslint . --ext .ts --fix`                 | Checks for style/potential errors and attempts auto-fixing.     |
| prettier         |`prettier "**/*.{js,jsx,json,md,ts}" --check` | Checks code formatting against Prettier standards.              |
| prettier:fix     |`prettier "**/*.{js,jsx,json,md,ts}" --write` | Reformats code according to Prettier standards.                 |
