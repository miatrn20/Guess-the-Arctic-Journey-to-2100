# ❄️ Guess the Arctic: A Journey to 2100

**DSC 106 — Interactive Climate Visualization**

An immersive, interactive climate-storytelling website where readers guess how much the Arctic will warm, compare their prediction with CMIP6 projections, explore a polar map, and compare regional warming across emissions scenarios.

## Current status

🚧 **Concept prototype / work in progress**, not a completed climate-data visualization. The "race to +3°C" chart is built with D3.js (loaded from a CDN). The polar map and year slider are still placeholders and will become real CMIP6 D3 views.

## How to run locally

1. Download or clone the repository.
2. Open the folder in VS Code.
3. For a simple first preview, open `index.html` in a browser. For data-loading work, use a local server (e.g., VS Code Live Server or `python3 -m http.server 8000`) and visit `http://localhost:8000`.
4. No install step. D3 v7 loads from jsDelivr, so you need internet.

## Repository structure

```text
Guess-the-Arctic-Journey-to-2100/   (site files live at repo root for GitHub Pages)
├── index.html          # Five-page-chapter layout
├── css/
│   └── styles.css      # Colors, layout, responsive styles
├── js/
│   └── main.js         # Prototype interactions (refactor as features grow)
├── data/
│   └── README.md       # Data provenance and future exports
├── docs/
│   └── PROJECT_PLAN.md # Team scope and division of work
├── CONTRIBUTING.md     # Branch and pull-request workflow
└── README.md
```

## Planned visualizations

| Component | Current prototype | Planned real implementation |
|---|---|---|
| Guess the warming | End-of-century slider/drag guess + reveal | D3 freehand trajectory & actual time-series comparison |
| Arctic time machine | Static polar illustration; year label changes | D3 geographic polar heatmap updating with year/scenario |
| Regional discovery | Description selector and end-period comparison | Linked regional time-series charts with shared hover |
| Race to +3°C | Scenario-switched milestone plot | Verified year-to-threshold definitions and explanatory tooltips |

## Data and model

Project proposal: CanESM5 (r1i1p1f1), CMIP6 near-surface air temperature (`tas`), 1995–2014 baseline, latitude-weighted means, Arctic north of 66.5°N. Scenarios: SSP1-2.6, SSP2-4.5, SSP5-8.5. Example end-century Arctic values in the proposal: +6.2°C, +9.2°C, +14.3°C (2081–2100). These are **one model's projections**, not universal climate forecasts.

See `data/README.md` for validation requirements. No real time-varying gridded climate files are included in this starter.

## Deployment

GitHub Pages → **Settings** → **Pages** → **Deploy from a branch** → `main` → `/ (root)` → **Save**. A public repo is generally simplest with GitHub Free. Site URL will follow `https://miatrn20.github.io/Guess-the-Arctic-Journey-to-2100/` after successful deployment.

## Team workflow

Please read [CONTRIBUTING.md](CONTRIBUTING.md) before editing. Each teammate should work on a separate branch and open a pull request; avoid direct commits to `main` after initial setup.

## Credits

Course: DSC 106. Team: Patrick Wu, Hannah Tran, Yuki Saeli, Mia Tran. Climate data source: CMIP6 public archive (Google Cloud). Visualizations and all claims must be validated before release.
