# Syncfusion EJ2 Angular Sample (Browser-based)

This repository demonstrates how to use Syncfusion Essential JS 2 (EJ2) Angular UI components in a lightweight, browser-based development workflow. The sample is configured with the EJ2 Grid package and focuses on installing dependencies, running a local dev server, and building the app for production. It is designed to be simple, professional, and easy to follow, without any device or mobile-specific steps.

## Overview
- Framework: Angular (v5 as used in this sample)
- Tooling: Ionic App Scripts dev server for quick local preview in a browser
- Language: TypeScript
- UI Library: Syncfusion Essential JS 2 for Angular (EJ2)
- Example Component: EJ2 Grid (`@syncfusion/ej2-ng-grids`)

The repository keeps dependency versions aligned with the Angular 5 toolchain to minimize compatibility issues. You can run and test everything in a desktop browser.

## Prerequisites
- Node.js: Prefer 8.x or 10.x for best compatibility with Angular 5-era tooling
- npm: Prefer 5.x or 6.x

Tip: If you see install/build warnings with newer Node.js versions, use a Node version manager (such as nvm on macOS/Linux or nvm-windows on Windows) and switch to Node 10.x before running the steps below.

## Quick Start
1) Install dependencies
- From the project root, run:
  - `npm install`

2) Start the local development server (browser preview)
- Run:
  - `npm start`
- The terminal prints a local URL. Open it in your desktop browser to view the app.

3) Build a production bundle
- Run:
  - `npm run build`
- The optimized output is emitted to the `www/` folder.

## Project Scripts
- `npm start` — Launches a local dev server with live reload using Ionic App Scripts (for browser use only in this sample).
- `npm run build` — Produces a production-ready bundle under `www/`.
- `npm run clean` — Cleans build artifacts.
- `npm run lint` — Lints the project using Ionic App Scripts.

## Using Syncfusion EJ2 Components
This sample includes the EJ2 Grid. To use additional EJ2 Angular components:
- Install the package you need. Examples:
  - Buttons: `@syncfusion/ej2-angular-buttons`
  - Inputs: `@syncfusion/ej2-angular-inputs`
  - Calendars: `@syncfusion/ej2-angular-calendars`
- Import the corresponding Angular module into your feature or app module and add it to the `imports` array.
- Reference the component selector in your templates.

Documentation
- Getting Started with EJ2 Angular: https://ej2.syncfusion.com/angular/documentation/getting-started/angular-cli
- All EJ2 Angular Components: https://ej2.syncfusion.com/angular/documentation/

Version note
- This sample uses the historic `@syncfusion/ej2-ng-...` package names aligned with Angular 5. Modern Angular projects typically use `@syncfusion/ej2-angular-...`. If you plan to upgrade Angular, migrate packages accordingly and update peer dependencies (Angular, RxJS, TypeScript, zone.js).

## Project Structure (high level)
- `src/` — Application source code (components, modules, styles)
- `package.json` — Scripts and dependencies
- `www/` — Generated production build output (after `npm run build`)

## Troubleshooting
- Install warnings or peer dependency conflicts
  - Use Node 10.x and npm 6.x for a smoother install. Clear caches if needed (`npm cache verify`).
- Blank screen in the browser
  - Check the terminal/browser console for template or module import errors. Ensure all EJ2 modules used in templates are imported in the corresponding Angular module.
- Styling issues
  - Verify the EJ2 theme CSS is referenced in your app (if applicable for the components you add).

## FAQ
- Is this project intended for mobile/device deployment?
  - No. This sample focuses on a browser-based development flow only.
- Can I upgrade to newer Angular versions?
  - Yes, but perform upgrades incrementally and align all related dependencies, including Syncfusion EJ2 packages and Angular tooling.

## License
This sample is provided for demonstration purposes only. Syncfusion Essential JS 2 packages are subject to their respective licensing terms: https://www.syncfusion.com/licensing

## Support
For technical questions related to Syncfusion EJ2 Angular components, visit: https://www.syncfusion.com/support
