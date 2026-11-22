# GitHub Profile README — Maintenance & Workflow Notes

Repository source for **MD Saidur Rahman Bhuyan** (`https://github.com/saidur1004/saidur1004`).

## Project Structure

```text
saidur-github-profile/
├── README.md                  # Primary GitHub Profile README (editorial light/dark theme)
├── README-preview.md          # Maintenance and workflow notes
├── assets/
│   ├── banner.svg             # Light-theme editorial masthead (#F5F3EF / #172033)
│   ├── banner-dark.svg        # Dark-theme editorial masthead (#172033 / #F8FAFC)
│   └── footer.svg             # Minimal hairline footer divider
└── .github/
    └── workflows/
        └── snake.yml          # GitHub Actions workflow for contribution snake SVGs
```

## Featured Live Applications

1. **EzyDash** — Google Play (`com.ezydash`) & Apple App Store (`id6749002165`)
2. **ChugChain** — Google Play (`com.chugchain.app`) & Apple App Store (`id6811016657`)
3. **Energy Consumer** — Google Play (`app.energhxplus.consumer`) & Apple App Store (`id6814630663`)
4. **Energy Developer** — Google Play (`app.energhxplus.developer`) & Apple App Store (`id6814628868`)
5. **Energy Server** — Google Play (`app.energhxplus.server`) & Apple App Store (`id6814631137`)
6. **EnerghxPLUS Admin** — Google Play (`app.energhxplus.admin`) & Apple App Store (`id6821299508`)

## Technical Notes

- **Theme Compatibility:** Uses GitHub's native `<picture>` + `prefers-color-scheme` elements for Light and Dark modes.
- **Skillicons `srcset` Encoding:** Commas inside `<source srcset="...">` URLs are percent-encoded as `%2C` so browsers do not treat them as `srcset` URL candidate delimiters.
- **Contribution Snake:** `.github/workflows/snake.yml` generates `github-contribution-grid-snake.svg` and `github-contribution-grid-snake-dark.svg` on the `output` branch.
