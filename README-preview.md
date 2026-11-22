# GitHub Profile README — Preview & Publishing Notes

This directory contains the GitHub Profile repository source for **MD Saidur Rahman Bhuyan** (`saidur1004`).

## Repository Structure

```text
saidur-github-profile/
├── README.md                  # Primary GitHub Profile README
├── README-preview.md          # Local preview, verification, and setup notes
├── assets/
│   ├── banner.svg             # Custom dark-theme-friendly SVG hero banner
│   └── footer.svg             # Custom SVG wave footer accent
└── .github/
    └── workflows/
        └── snake.yml          # GitHub Actions workflow for contribution snake SVG
```

## How GitHub Profile READMEs Work

1. Create a **public** repository named **`saidur1004`** (matching your exact GitHub username `saidur1004`).
2. Push this repository so `README.md` lives at the root of `github.com/saidur1004/saidur1004` on the `main` branch.
3. GitHub automatically renders `README.md` at the top of `https://github.com/saidur1004`.

## Enabling the Contribution Snake Animation

The workflow in `.github/workflows/snake.yml` uses `Platane/snk@v3` with the default `GITHUB_TOKEN` (no personal access token required):

1. Push the repository to `https://github.com/saidur1004/saidur1004`.
2. Open **Actions** -> **Generate Contribution Snake** -> **Run workflow** (or wait for the scheduled run).
3. Confirm that the `output` branch now contains `github-contribution-grid-snake.svg` and `github-contribution-grid-snake-dark.svg`.
4. Uncomment the `<!-- Contribution Snake -->` `<picture>` block in `README.md` and commit/push the update.
