# Governance Demo Builder

**Holistic AI · Sales enablement**

Governance Demo Builder turns buyer questions into a timed sales demo runbook. Each segment links a question to an action the presenter will show and the proof point the buyer should take away.

## Why I built it

I built this around my work developing scripts, FAQs, decks, and product demos for the 2025/26 Holistic AI platform launch. It demonstrates how I would structure a buyer-specific story around the product actions that make it credible.

## Try the sample

1. Open the sample for a governance operations lead. The three segments total **11 minutes** against a **15-minute** meeting budget.
2. Lower the budget to **10 minutes** to see where the walkthrough stands. Shorten a segment or add one for a buyer objection and watch the total update.
3. Capture the buyer question, action, and proof point for each step. Move a segment from **Draft** to **Rehearsed** or **Ready** as you prepare.
4. Click **Download Markdown** for a presenter runbook with the segment timings and preparation status.

The time budget applies to the demo segments. Include time for discussion in your plan if the call needs it.

## Run locally

Download the repository ZIP or clone it, then open `index.html` in a modern browser.

```sh
git clone https://github.com/johnmir94/governance-demo-builder.git
cd governance-demo-builder
```

The app uses HTML, CSS, and JavaScript and runs entirely in the browser without an account or backend. Sample data is fictional. Edits stay in the current tab, so download the Markdown before reloading or closing it.

## Source files

| File | Role |
| --- | --- |
| `index.html` | Workspace layout and controls |
| `style.css` | Responsive styling |
| `data.js` | Fictional sample workspace |
| `app.js` | Editing, validation, summaries, and Markdown export |
