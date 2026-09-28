# Dino Game

A standalone web version of the classic Chromium T-Rex runner game featuring an automated player script and GitHub Pages deployment.

## Features

- **Self-contained**: Entire game, sprite sheets, and audio assets bundled in a single [`index.html`](index.html).
- **Auto-Play Bot**: Includes an autonomous jumping algorithm that calculates obstacle approach times, jumps obstacles automatically, and handles restarts.
- **Dark Mode Support**: Adapts automatically to system light/dark theme preferences.
- **Score Tracking**: Saves high scores locally using browser `localStorage`.
- **Automated Deployment**: Includes a GitHub Actions workflow ([`.github/workflows/deploy.yml`](.github/workflows/deploy.yml)) to publish the game directly to GitHub Pages on push to `main`.

## Running Locally

Simply open [`index.html`](index.html) in any modern web browser:

```bash
open index.html
```

Or serve with any static web server:

```bash
npx serve .
# or
python3 -m http.server
```

## Deployment

The project is deployed to GitHub Pages automatically via GitHub Actions:

1. In your GitHub repository, navigate to **Settings** > **Pages**.
2. Under **Build and deployment**, select **GitHub Actions** as the source.
3. Every push to the `main` branch triggers the [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml) workflow to publish the site.
