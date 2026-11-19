# Journey to 2100 — project plan

## Goal

Turn the six static proposal figures into one playful, immersive D3.js climate narrative. Readers should make a prediction, reveal model results, explore the Arctic through time, compare regional trends, and learn when regions cross +3°C.

## Five chapters

1. **The Invitation:** illustrated Arctic landing page and start button.
2. **Draw Your Future:** guess a temperature anomaly trajectory before revealing a CMIP6 projection.
3. **Arctic Time Machine:** polar projection, 2015–2100 year slider, scenario controls, map tooltip and linked line chart.
4. **One Planet, Different Futures:** linked small multiples for Arctic, northern midlatitudes, tropics, southern midlatitudes and optionally global average.
5. **Race to +3°C:** scenario-filterable year-to-threshold dot plot; show “not by 2100” when relevant.

## UX & visual language

- Polar night `#10283F`, glacier blue `#78DCE8`, coral `#F7AA87`, snow cream `#F8EDCF`.
- Playful editorial typography and scenic transitions; charts remain accurate and accessible.
- Shared `selectedYear`, `selectedScenario`, `selectedRegion` state.
- Provide mobile, keyboard and reduced-motion alternatives.

## Milestones

**Prototype:** working landing page, initial interactive guess/reveal, visual design, description of remaining D3 implementation.

**Final:** working D3 guess chart, real scenario/year polar heatmap, linked regional time-series, validated +3°C chart, captions/methods and GitHub Pages release.

## Important scientific note

The proposal's 2081–2100 CanESM5 Arctic anomaly values are 6.2°C, 9.2°C and 14.3°C. One model may overstate or understate the multi-model ensemble outcome. Always call these projections and cite the underlying dataset.
