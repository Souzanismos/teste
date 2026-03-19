# teste

Recommended IDE Setup
VS Code + Vue (Official) (and disable Vetur).

Recommended Browser Setup
Chromium-based browsers (Chrome, Edge, Brave, etc.):
Vue.js devtools
Turn on Custom Object Formatter in Chrome DevTools
Firefox:
Vue.js devtools
Turn on Custom Object Formatter in Firefox DevTools
Type Support for .vue Imports in TS
TypeScript cannot handle type information for .vue imports by default, so we replace the tsc CLI with vue-tsc for type checking. In editors, we need Volar to make the TypeScript language service aware of .vue types.

Customize configuration
See Vite Configuration Reference.

Project Setup
npm install
Compile and Hot-Reload for Development
npm run dev
Type-Check, Compile and Minify for Production
npm run build
Run Unit Tests with Vitest
npm run test:unit
Run End-to-End Tests with Playwright
# Install browsers for the first run
npx playwright install

# When testing on CI, must build the project first
npm run build

# Runs the end-to-end tests
npm run test:e2e
# Runs the tests only on Chromium
npm run test:e2e -- --project=chromium
# Runs the tests of a specific file
npm run test:e2e -- tests/example.spec.ts
# Runs the tests in debug mode
npm run test:e2e -- --debug
Lint with ESLint
npm run lint
