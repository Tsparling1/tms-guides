# TMS Solutions Member Guides

A lightweight web app for browsing and downloading TMS Solutions member guide PDFs, organized by category.

## Quick Start

```bash
cd tms-guides
npm install
npm start
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

## Adding Guides

1. Create a subfolder inside `public/guides/` for each category:
   ```
   public/guides/onboarding/
   public/guides/billing/
   public/guides/compliance/
   ```
2. Drop `.pdf` files into the appropriate folder.
3. The app auto-discovers them — no configuration needed.

## Development

```bash
npm run dev   # starts server with nodemon (auto-restart on changes)
```

## Configuration

| Variable | Default | Description             |
|----------|---------|-------------------------|
| `PORT`   | `3000`  | Port the server runs on |

## Tech Stack
- **Backend**: Node.js + Express (static file server + minimal REST API)
- **Frontend**: Vanilla HTML/CSS/JS (no build step)
- **PDF storage**: Local filesystem under `public/guides/`
