# AGENTS.md

## Stack

- Vite 7 + React 19, JSX (no TypeScript)
- ESLint 9 flat config, no formatter/prettier
- No test framework, no typecheck, no CI

## Commands

```bash
npm install        # install deps
npm run dev        # Vite dev server → http://localhost:5173
npm run build      # production build → dist/
npm run lint       # eslint .
npm run preview    # preview prod build locally
```

No test or typecheck commands exist. `npm run lint` is the only verification step.

## ESLint notes

- Ignores `dist/`
- `no-unused-vars` allows names matching `^[A-Z_]` (component names, constants)

## Project structure

All app code lives in `src/App.jsx` — single-component app with inline state, no routing, no component decomposition. `src/main.jsx` is the entry point.

## Notes

- Freelance Work seed entry has been corrected to `type: "income"` (was incorrectly `type: "expense"`)
- All state and UI live in one component
