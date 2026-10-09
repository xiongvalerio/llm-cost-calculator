# LLM Cost Calculator

**Estimate what a request, a day, or a month of inference actually costs.**

A single-page tool for anyone who runs or resells AI APIs. Plug in your token
volumes and per-million prices, get the real number, and compare models side by
side.

## What it does

- Token → cost math for input, cached input, and output tokens
- Per-request, per-day, and per-month projections
- Preset pricing for popular models (editable)
- Side-by-side comparison of two models
- Margin calculator for resellers: enter your sell price, see your take
- Everything runs in the browser, nothing is uploaded

## Why

Reselling or proxying AI APIs without tracking unit economics is how people lose
money. This tool answers the only question that matters:

> If I charge X and my upstream costs Y, what do I keep?

## Usage

Open `index.html` in a browser. No install, no build, no account.

```
git clone https://github.com/xiongvalerio/llm-cost-calculator.git
cd llm-cost-calculator
python -m http.server 8080
# open http://localhost:8080
```

## Dataset

`data/models.json` ships a snapshot of 656 models with their advertised price
floors (source: AntSeedStats, CC BY 4.0). It is a convenience reference for
seeding your own pricing tables — check the source before relying on it.

## License

MIT
