# GitHub Profile README — Maintenance & Workflow Notes

Repository source for **MD Saidur Rahman Bhuyan** (`https://github.com/saidur1004/saidur1004`).

## Project Structure

```text
saidur-github-profile/
├── README.md                  # Primary GitHub Profile README (editorial light/dark theme)
├── README-preview.md          # Maintenance and workflow notes
├── assets/
│   ├── banner.svg             # Light-theme editorial header banner (#F5F3EF / #172033)
│   ├── banner-dark.svg        # Dark-theme editorial header banner (#172033 / #F8FAFC)
│   └── footer.svg             # Minimal hairline footer divider
└── .github/
    └── workflows/
        └── snake.yml          # GitHub Actions workflow for contribution snake SVGs
```

## Theme Compatibility

`README.md` uses GitHub's native `<picture>` + `prefers-color-scheme` elements so the hero banner, skill icons, statistics cards, streak card, and contribution activity graph adapt automatically to both **GitHub Light** and **GitHub Dark** themes.

## Contribution Snake Workflow

`.github/workflows/snake.yml` runs on schedule (`0 0 * * *`), on push to `main`, and via manual `workflow_dispatch` using `GITHUB_TOKEN` with `contents: write` permission.

Once the `output` branch contains `github-contribution-grid-snake.svg` and `github-contribution-grid-snake-dark.svg`, uncomment the `<!-- Contribution Snake -->` `<picture>` block in `README.md`.
