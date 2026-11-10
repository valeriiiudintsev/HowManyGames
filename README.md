# HowManyGames

A game catalog and personal game tracker built with React, TypeScript, Redux Toolkit, Material UI, and Vite. Browse and filter games, manage planned/playing/completed lists, write reviews, and view statistics. Includes screens for editing games, developers, publishers, genres, tags, and platforms.

## Run

Requires Node.js and npm, plus a running compatible backend (not included in this repository).

```sh
npm ci
```

Set `VITE_API` in `.env.local` to your backend's base URL, without a trailing slash. For example, if it runs on port 5000:

```dotenv
VITE_API=http://localhost:5000
```

The client appends API paths such as `/api/Game` to this URL.

```sh
npm run dev
```

Open the local URL printed by Vite (normally `http://localhost:5173`).

## Build

```sh
npm run build
npm run preview
```

The build runs TypeScript checks and writes production assets to `dist/`. The preview command serves that build locally. Set `VITE_API` before building; it is embedded in the frontend bundle.
