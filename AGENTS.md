# jacobenders

Personal webpage at https://jacobenders.com.

## Commands

```sh
just fmt        # prettier --write **/*.html
nix develop     # enter dev shell (php, prettier, just)
```

## Constraints

- Every page **must** have a "generated with AI" warning.
- Style: very pretty purple gradients, futuristic monospace fonts.

## How it works

- Single-page static site in `src/` — no framework, no build step.
- Tailwind CSS loaded via CDN `<script>` in `index.html`.
- Deployed to GitHub Pages automatically on push to `main` via `.github/workflows/static.yml` (uploads `src/` directory).
