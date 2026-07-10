# Colima Manager

A desktop application for managing [Colima](https://github.com/colima-dev/colima) built with Tauri 2, React 19, TypeScript, and Rust.

> Before making any changes, read `AGENTS.md`. It is the single source of truth for repository conventions, skills, and workflow.

## Repo Overview

- `src/` — React frontend. Entry point: `main.tsx`
- `src-tauri/` — Rust backend and Tauri integration
- `public/` — Static assets
- `AGENTS.md` — Repository-specific guidance for skills and workflows

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) with [pnpm](https://pnpm.io/)
- [Rust](https://www.rust-lang.org/tools/install)
- [Xcode](https://developer.apple.com/xcode/) (macOS)

### Install

```bash
pnpm install
```

### Useful Commands

Use `pnpm` for all commands in this repository.

- `pnpm dev` — Start the Vite dev server on port `1420`
- `pnpm tauri dev` — Run the full desktop app in development
- `pnpm build` — Build the frontend and output production assets
- `pnpm tauri build` — Package the desktop app
- `pnpm build:macos` — Build a macOS DMG installer
- `pnpm lint:check` — Check lint and formatting
- `pnpm lint:fix` — Fix lint and formatting issues

## Repository Notes

- Frontend dev server port: `1420`
- `src-tauri/**` is excluded from Vite file watching during `tauri dev`
- `TAURI_DEV_HOST` can override the Tauri dev host
- Rust crate name: `colima_manager_lib`

## Where to Look First

Read `AGENTS.md` before doing anything else in this repository. It contains the repo-specific guidance for skills, conventions, and workflow.
