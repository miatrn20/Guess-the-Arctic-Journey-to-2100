# Collaborating on Guess the Arctic

## Recommended team workflow

**Rule:** One shared repository, one feature branch per task, review through pull requests.

1. Clone the repo (GitHub Desktop: **File → Clone repository**) and open in VS Code.
2. Fetch / pull the latest `main` branch.
3. Create your feature branch with a descriptive name, such as `feature/guess-chart`, `feature/polar-map`, `feature/region-charts`, or `feature/site-design`.
4. Make small focused changes and preview locally.
5. Commit with descriptive messages (`Add scenario buttons to guess chart`).
6. Push your branch to GitHub.
7. Open a **Pull request** targeting `main`; ask one teammate to review; merge after confirming the website works.
8. Pull updated `main` before starting the next task.

## Suggested ownership

- **Prediction interaction:** draw/reveal flow, accuracy comparison, D3 line/drag chart.
- **Polar visualization:** map projection, real gridded data, time/scenario controls.
- **Regional comparisons:** synchronized multi-chart hover, +3°C milestones.
- **Layout & integration:** design system, navigation, deployment, accessibility, shared state.

Confirm actual assignments as a team. All members review data definitions, testing and interpretation.

## Avoid merge conflicts

Current JavaScript is in one `js/main.js` file. Before working on four features simultaneously, agree on interfaces and progressively split code into modules (`js/guess-chart.js`, `js/polar-map.js`, `js/region-charts.js`, `js/threshold.js`). Keep shared selected year and scenario state in one place. Coordinate before changing `index.html` or `css/styles.css`.

## Definition of done for each pull request

- [ ] Interactive functionality works on desktop.
- [ ] Labels, baselines and units are correct.
- [ ] Existing features still work; no console errors.
- [ ] Works on a narrow mobile viewport or documents a known limitation.
- [ ] Describes changes and includes screenshot/video if visual.
- [ ] Another teammate has reviewed the pull request.

## Example Git commands (optional)

```bash
git clone https://github.com/YOUR-USERNAME/guess-the-arctic.git
cd guess-the-arctic
git checkout -b feature/guess-chart
# edit in VS Code
git add .
git commit -m "Build D3 guess chart"
git push -u origin feature/guess-chart
```

Open a pull request on GitHub to merge your branch into `main`.
