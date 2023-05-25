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

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Eslint

# Setup

You can also manually set up ESLint in your project.

- Install eslint project in your project
  ```bash
  npm install --save-dev eslint (or)
  npm i -D elsint
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
