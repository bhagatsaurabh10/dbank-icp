# DBank

DBank is a small Internet Computer banking demo built with Motoko and JavaScript. It was created as a course project to practice canister development, frontend-to-canister calls, and local deployment with the DFINITY SDK.

## Features

- Motoko backend canister that stores the account balance as stable state
- Top-up and withdrawal actions with a simple overdraft check
- Compound interest calculation based on elapsed time
- Webpack frontend that calls the canister methods and updates the UI

## Tech Stack

- Motoko
- Internet Computer / DFINITY SDK
- JavaScript
- Webpack
- HTML/CSS

## Getting Started

Install dependencies:

```bash
npm install
```

Start the local Internet Computer replica:

```bash
dfx start --clean
```

In another terminal, deploy the canisters:

```bash
dfx deploy
```

Start the frontend development server:

```bash
npm start
```

The app will run through the Webpack dev server and proxy canister calls to the local replica.

## Project Structure

```text
src/dbank/main.mo                # Motoko backend canister
src/dbank_assets/src/index.js    # Frontend canister calls
src/dbank_assets/src/index.html  # App markup
src/dbank_assets/assets/         # Static assets and styles
dfx.json                         # Canister configuration
```

## Notes

This is a learning project and is not intended for real financial use. The balance and interest logic are simplified to demonstrate core Internet Computer concepts.
