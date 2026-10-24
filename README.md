# Petri

A small browser-based microbial ecosystem. Cells forage, consume energy, divide, inherit mutations, and die. Speed, size, and efficiency influence survival. This is an exploratory toy model, not a scientific simulator.

## Run

Requires Python 3; no packages or build step are needed.

```sh
cd /workspace/test-sim-game
python3 -m http.server 8000 --bind 0.0.0.0
```

Open the served page in a browser. Click a microbe to inspect its energy, age, generation, and inherited size, speed, and efficiency. Trait changes are shown relative to its parent and founding ancestor; use Follow a living descendant to explore its lineage. Enable Place nutrients, then click the dish to add food at a chosen location. Turn it off (or press Escape) to return to inspection. Ordinary inspection clicks never add food. Use the controls to pause, accelerate time, adjust food supply, introduce cells, or reset. Population is capped at 350 and food at 650 to keep the simulation responsive. Fonts fall back to system fonts if Google Fonts is unavailable.

## Files

- `index.html`: interface
- `style.css`: responsive styling
- `app.js`: canvas rendering and simulation

No credentials, external services, or database are required.
