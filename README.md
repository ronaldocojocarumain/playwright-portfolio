# Playwright Portfolio

E2E testing framework with Playwright and TypeScript for [Sauce Demo](https://www.saucedemo.com).

![Playwright Tests](https://github.com/ronaldocojocarumain/playwright-portfolio/actions/workflows/playwright.yml/badge.svg)

## Included tests

**Login (login.spec.ts)**
- Data-driven with JSON: locked out user, wrong password, empty fields

**Purchase flow (saucedemo.spec.ts)**
- Sorting by price (dropdown)
- Opening a product in a new tab
- Shopping cart
- Shipping data
- Checkout overview
- Order completed

## Technical features
- Page Object Model (POM)
- Data-driven testing with JSON + forEach
- Tests organized in suites with test.describe
- actionTimeout configured (10s)
- Screenshot and video recorded on failure
- CI/CD with GitHub Actions on every push

## Tech stack
- [Playwright](https://playwright.dev/) v1.x
- TypeScript
- Page Object Model

## Running the tests

Install dependencies:

```
npm install
npx playwright install chromium
```

All tests:

```
npx playwright test
```

Chromium only:

```
npx playwright test --project=chromium
```

View the report:

```
npx playwright show-report
```
