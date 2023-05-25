This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

# Eslint

### What is Eslint?

Eslint is a configurable tool, which helps to identify and fix problems in your javascript code. Problems can be anything from potential bugs, to following best practices, to styling issues.

### Setup

You can also manually set up ESLint in your project.

- Install eslint project in your project
  ```bash
  npm install --save-dev eslint (or) npm i -D elsint
  ```
- Create a .eslintrc.(js/json) file in your root folder

  ```bash
  touch .eslintrc or

  touch .eslintrc.js or

  touch .eslintrc.json
  ```

- Add following basic code to your .eslintrc file
  ```bash
  module.exports = {
    "env": {
        "browser": true,
        "es2021": true
    },
    "extends": "eslint:recommended",
    "parserOptions": {
        "ecmaVersion": "latest",
        "sourceType": "module"
    },
  }
  ```
- Run the following command to check linting errors
  ```bash
  npx eslint project-dir/ file1.js
  ```

### Core concepts

#### rules

Rules are building blocks of eslint. A rule validates if your code meets certain expectation or not, and what to do if doesn't meet the expectation.
Each rule has a unique identifier and can be configured to report an error, a warning or turned off. You constumized the rule based on your project coding standards or use popular preset configurations like "eslint:recommended" or "airbnb" that come bundled with a set of commonly used rules.

#### Configurations

- Configurations file is a place where all your built in rules, plugins, custom rules and shareable configs exist
- Shareable conguration is a npm module, which can be share to any project

#### Plugins

A ESLint plugin is a npm module, which contain set of rules, configurations, preprocessors and environments. Plugins can be used to enforce a style guide to support Javascript extensions like Typescript, library (React), framework (Angular) etc.
