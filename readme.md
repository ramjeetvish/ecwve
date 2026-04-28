# ECWVE Content Workspace

This repository is a Windows-first local workspace for ECWVE content development. It provides the local dev server, repository structure, and used to work on HTML modules, shared assets, and reusable interaction templates.

## Repository Purpose

Use this repository when you need to:

- run the local ECWVE development server
- work on HTML module content and shared assets
- keep production-ready project files tracked in Git
- keep temporary test material out of Git

## What Lives Here

- Project content goes in `virtual_env/`
- Reference and test material can stay in `virtual_env/tests/`
- Shared tooling and local server configuration live at the repository root

## Quick Start

1. Clone the repository:

	```powershell
	git clone https://github.com/ramjeetvish/ecwve.git
	cd ecwve
	```

2. Install dependencies:

	```powershell
	npm install
	```

3. Add your project files under `virtual_env/`.

4. Start the local dev server:

	```powershell
	npm run dev
	```

5. Open the configured start page in the local server. The current default path is `mod01/01s00l0000.html`.

## Requirements

- Node.js 20.11 or newer


## Folder Rules

- Use `virtual_env/` for tracked project content
- Keep tooling and package configuration at the repository root

## Daily Workflow

1. Start the dev server with `npm run dev`.
2. Open the page you are working on.
3. Edit files in `virtual_env/`.
4. Auto refresh and verify the affected module or shared asset.
5. If you changed shared CSS, JavaScript, or includes, test more than one page before finishing.

## Troubleshooting

If `npm run dev` fails:

- confirm Node.js 20.11 or newer is installed
- run `npm install` again from the repository root
- verify your project files exist under `virtual_env/`
- check that the configured start page exists for your project

If the browser opens but the page is missing:

- confirm your content package includes the module referenced by `startPath`
- update `package.json` if your entry page is different
