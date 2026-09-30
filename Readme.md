# Task: ReactJS - Hello World

## Problem Statement
A basic "Hello World" React application.

## Problem Description
A simple React application that displays the text **"Hello, World!"** on
the screen.

## Tooling
Scaffolded with **Vite** (`npm create vite@latest -- --template react`).

## Project structure
```
hello-world/
├── index.html
├── package.json
├── vite.config.js
├── public/
│   └── favicon.svg
└── src/
    ├── main.jsx      # React entry point, mounts <App />
    ├── App.jsx        # Renders "Hello, World!"
    ├── App.css        # Centers the heading on the screen
    └── index.css      # Minimal global reset
```

`App.jsx` is intentionally minimal:

```jsx
function App() {
  return (
    <div className="hello-container">
      <h1>Hello, World!</h1>
    </div>
  )
}
```

## How to run
```bash
npm install
npm run dev
```
Then open the URL Vite prints (typically `http://localhost:5173`) in your
browser — it will display **"Hello, World!"** centered on the page.

## How to build for deployment
```bash
npm run build
```
This produces a static `dist/` folder that can be deployed to any static
host (Netlify, Vercel, GitHub Pages, etc.).

## Verification
`npm run build` and `npm run lint` were both run before submission and
passed with 0 errors/warnings.

Note: `node_modules/` is not included in this submission (regenerate it
with `npm install`) as instructed.
