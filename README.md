# Governance Demo Builder

Use the builder to prepare a sales walkthrough from a buyer scenario. Each segment connects a question to a product action and the evidence that action should establish. The meeting budget helps the presenter decide which segments can fit.

## Run locally

Clone the repository or use **Code → Download ZIP** on GitHub. Open `index.html` in a modern browser. There’s no install, build step, or account required.

```sh
git clone https://github.com/johnmir94/governance-demo-builder.git
cd governance-demo-builder
```

## Sample workflow

1. Open the sample for a governance operations lead. The three segments total **11 minutes** against a **15-minute** meeting budget.
2. Lower the budget to **10 minutes** to see where the walkthrough stands. Shorten a segment or add one for a buyer objection and watch the total update.
3. Capture the buyer question, action, and proof point for each step. Move a segment from **Draft** to **Rehearsed** or **Ready** as you prepare.
4. Click **Download Markdown** for a presenter runbook with the segment timings and preparation status.

## Workspace fields

| Field | What it captures |
| --- | --- |
| Buyer and desired outcome | The audience and what the meeting should establish |
| Demo segment | A named step in the walkthrough |
| Buyer question | The objection or decision the step addresses |
| Action and proof point | What to show and what it demonstrates |
| Minutes and status | Planned duration and preparation state |

## How it works

The app adds the duration of all segments and compares it with the meeting budget. If the total exceeds the budget, the summary shows the difference. Status is tracked independently as Draft, Rehearsed, or Ready. The time calculation uses the minutes entered for each segment. Add a discussion segment if time for questions needs to be reserved.

### Worked example

The sample allocates two minutes to framing the buyer scenario, five to model registration, and four to reviewing the audit record. That leaves four minutes in a 15-minute slot. Lower the budget to 10 minutes to see a one-minute overrun.

## Export and data handling

Markdown includes the buyer outcome, timing summary, and each segment’s question, action, minutes, and preparation status.

Processing runs in the browser. The app has no backend and keeps edits in memory. Reloading reopens the fictional sample. Download the Markdown before closing the tab if you need a copy of your work.

## Files and checks

| File | Role |
| --- | --- |
| [`index.html`](index.html) | Workspace and controls |
| [`style.css`](style.css) | Responsive layout |
| [`data.js`](data.js) | Fictional seed data and field labels |
| [`app.js`](app.js) | Editing, validation, summaries, and Markdown export |

Run JavaScript syntax checks with Node.js. Use the sample workflow above for a manual check of editing, summary updates, and the export.

```sh
node --check app.js
node --check data.js
```

## Project context

The workflow draws on sales enablement for the Holistic AI platform launch, including scripts, FAQs, decks, and product demos. The sample is fictional and uses no internal employer materials or customer records.
