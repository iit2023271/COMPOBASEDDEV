# React Navbar Demo — Component-Based Development

A React demo site built around reusable components: a `Navbar` with routed pages (Home, About, Services, Contact) plus a `Card` component. A component-based-development exercise in React + React Router.

![Demo](screenshots/demo.png)

## Features

- **Navbar component** — site-wide navigation bar with links to every page
- **Routed pages** — Home, About, Services, Contact via React Router
- **Card component** — reusable card UI used across pages
- **Services page** — a longer services listing page

## Tech Stack

- React 18 + React Router 6 + Vite 4
- Plain CSS (no UI framework)

## How to Run

The runnable app lives in the nested project folder (it has the proper `src/` layout):

```bash
cd "component--main/react-navbar-main (1)/react-navbar-main"
npm install
npm run dev
```

Then open the URL Vite prints (usually `http://localhost:5173`).

## Notes

- **Honest layout note:** the flat files at the repo root do not run as-is — the root `index.html` points to `/src/main.jsx`, which does not exist at the root, and the root `App.jsx` imports from `./components/`, which is also not at the root. The working copy is the nested project under `component--main/`, and the screenshot above is from that copy.
- `App.js` at the root is a standalone login form that is not used — `main.jsx` imports `App.jsx`, so `App.js` is dead code.
