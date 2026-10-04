# jacobenders

Personal webpage at https://jacobenders.com.

## Commands

```sh
just fmt        # prettier --write **/*.html
nix develop     # enter dev shell (php, prettier, just)
```

## Constraints

- Every page **must** have a "generated with AI" warning.
- Style: plain, readable HTML with a simple system font stack. No gradients,
  animations, or effects.

## How it works

- Single-page static site in `src/` — no framework, no build step.
- Styling is a small inline `<style>` block in `index.html`, no CDN.
- Deployed to GitHub Pages automatically on push to `main` via `.github/workflows/static.yml` (uploads `src/` directory).
