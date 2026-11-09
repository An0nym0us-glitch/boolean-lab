# BooleanLab website

The promotional website for [BooleanLab](https://github.com/An0nym0us-glitch/logic-gates-lab),
a free, offline Windows app for building and simulating digital logic circuits.

The site is a single static page (`site/index.html`) with no build step. It includes:

- A live circuit in the hero: flip switches A and B, swap between the seven gates, and watch the wires and LED update.
- The app's own gate lessons, with a clickable truth table and a step-through player.
- A tour of the Learn, Build and Experiment modes using real screenshots.
- An interactive half adder with a live truth table and output expressions.
- Feature, simulation-engine, test-suite and build-from-source sections.

## Preview locally

```bash
python3 -m http.server -d site 8000
```

Then open http://localhost:8000.

## Hosting

`.github/workflows/pages.yml` publishes the `site/` folder to GitHub Pages on every push to the
default branch. If the first run cannot enable Pages on its own, open
**Settings → Pages**, set **Source** to **GitHub Actions**, and re-run the workflow.
