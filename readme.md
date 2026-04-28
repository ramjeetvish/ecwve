# ECWVE Content Package

This repository contains a modular browser-based learning package. It is intended for internal development and maintenance of HTML-based modules, shared assets, reusable interaction templates, and supporting files.

## About This Repo s

- A Windows-first local development setup
- Put Content under `virtual_env/`
- Shared CSS, JavaScript, media, and include files used across modules

## Requirements

- Windows
- Node.js 20.11 or newer
- npm

## Getting Started

Install dependencies from the repository root:

```powershell
npm install
```

Start the local development server:

```powershell
npm run dev
```

The dev server is configured in `package.json`. The current default start page is:

```text
mod01/01s00l0000.html
```

If the server prints a local URL instead of opening a browser automatically, use that URL and navigate to the configured start page.

## Daily Use

Use this repository when you need to:

- Preview module pages locally during content or asset changes
- Update shared styling, scripting, or layout includes
- Maintain reusable interaction templates
- Adjust files

For most work, the loop is:

1. Run `npm run dev`.
2. Open the affected page or module in the local server.
3. Edit the relevant HTML, CSS, JS, or media files.
4. Refresh and verify the affected flow.
5. If you changed shared assets, check more than one module before finishing.

## Working In The Repo
The tracked content package currently lives under `virtual_env/`.

### Module Content

Update module-specific pages inside the matching `virtual_env/` directory. Keep existing naming and relative-link conventions unless there is a deliberate migration plan.
