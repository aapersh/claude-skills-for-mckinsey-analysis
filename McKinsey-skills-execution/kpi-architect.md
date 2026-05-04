---
name: kpi-architect
description: Replace vanity metrics with the small set of KPIs that actually drive strategic decisions. Use when defining a new strategy's success measures, redesigning the management dashboard, or fixing a metrics system that is producing motion but not progress. Built around the KPI tree, leading-vs-lagging discipline, and target-setting rigor.
---

# KPI Architect

## Purpose

Build the metrics system that ties day-to-day operating activity to strategic outcomes — so that improvement at the bottom translates into result at the top, and so that leadership can detect drift early enough to act.

The deliverable is a KPI tree, not a dashboard. The dashboard is the artifact. The tree is the thinking.

## Governing Principle

**A KPI is only useful if it changes someone's behavior. If no one will act differently based on a metric, it is reporting, not management.**

Senior associates ruthlessly cull metrics that look impressive but drive no decision.

## The Three Categories of Strategic Metric

Every well-designed metrics system contains three layers, each serving a different purpose:

1. **North-star metric** — the single number that, if it moves, the strategy is succeeding (1 metric)
2. **Lagging outcome KPIs** — the financial and market results the strategy promises (3–5 metrics)
3. **Leading operational KPIs** — the inputs the team controls today that drive tomorrow's outcomes (5–10 metrics)

Anything that does not fit one of these three categories is operational reporting, not strategic measurement.

## Workflow

### Step 1 — Lock the north-star metric

The north-star is the single metric that best captures whether the strategy is working. It must satisfy four tests:

- **It moves with strategic success.** If the strategy works, this metric goes up. If not, it doesn't.
- **It is a measure of value delivered**, not activity performed.
- **It is countable and trackable in a reasonable cadence** (weekly or monthly, not annual).
- **It cannot be gamed in ways that hurt the business.**

Examples:
- Marketplace business: not "GMV," but "active buyer-seller pairs with repeat transactions"
- B2B SaaS: not "ARR," but "ARR from customers above the activation threshold"
- Retailer: not "store visits," but "revenue per active customer per month"

The north-star debate is worth 10× any other KPI debate. The team will optimize toward whatever it is. Pick carefully.

### Step 2 — Decompose the north-star arithmetically into a KPI tree

The KPI tree breaks the north-star into its multiplicative or additive components, then breaks those further. The tree is MECE at every level.

Example for a B2B SaaS north-star:

```
Activated ARR
├── New activated ARR
│   ├── New customers
│   │   ├── Leads × Lead-to-customer rate
│   │   └── Average new ACV
│   └── Activation rate of new customers
└── Existing activated ARR
    ├── Retained ARR (1 − gross churn rate)
    ├── Expansion ARR (% expanding × avg expansion size)
    └── Activation rate retention (existing activated → still activated)
```

Every leaf of the tree is now a candidate operational KPI.

### Step 3 — Select 3–5 lagging outcome KPIs

From the tree, pick the small set of metrics that directly express strategic outcomes. These are typically:

- A revenue or revenue-quality metric
- A profitability or unit economics metric
- A customer outcome metric (retention, satisfaction, lifetime value)
- A market position metric (share, share trend, win rate)
- A capability or asset metric, if the strategy depends on building one

Lagging KPIs answer "did we win?" — but they confirm yesterday's decisions, not tomorrow's.

### Step 4 — Identify the 5–10 leading operational KPIs

Leading KPIs are the inputs that, when moved this week, change the lagging outcomes next quarter. The test is: **if this metric improved by 20%, would it cause the lagging metrics to improve?**

For each leading KPI, document:

- **Definition:** the precise formula, including numerator, denominator, and time window
- **Owner:** the single named person accountable
- **Cadence:** how frequently it is reviewed (daily / weekly / monthly)
- **Driver:** what input behavior moves this metric

Leading metrics are where the operational work shows up. Without them, the strategy is unmeasurable until it has succeeded or failed — far too late.

### Step 5 — Set targets using triangulation

For each KPI, set a target using three reference points:

- **Historical performance:** what has been achievable in this organization?
- **External benchmark:** what do best-in-class peers achieve? (Public data, industry reports, hired benchmarks)
- **Strategic requirement:** what level does this KPI need to reach for the strategy's financial case to hold?

The target is the most ambitious of the three that the team can defend. Targets set only on history are too soft. Targets set only on the strategic case are detached from operational reality.

For each target, name:
- The threshold (the number)
- The timeline (when it must be hit)
- The trajectory (the quarterly path to get there, not just the endpoint)

### Step 6 — Define the action thresholds

For every KPI, predefine:

- **Green:** on or above plan trajectory — continue
- **Yellow:** drifting from plan — investigate and intervene at the operational level
- **Red:** materially off plan — escalate and reconsider at the strategic level
- **Black swan:** unprecedented movement (positive or negative) — special review

The thresholds must be set in advance. Setting them after the data lands is rationalization, not management.

### Step 7 — Test the system for gaming and proxy failure

For every KPI, run two failure tests:

- **Gaming test:** how would a clever team move this number without actually moving the underlying business outcome? If a credible gaming path exists, either fix the metric or pair it with a counterbalancing one.
- **Proxy failure test:** is this metric a proxy for what we actually care about? If so, when might the proxy decouple from the real outcome? (Example: NPS as a proxy for retention — works until customers are locked in by switching cost, at which point NPS drops while retention holds, and the system gives a false signal.)

Pair high-risk metrics with counterbalances:
- Speed metrics paired with quality metrics
- Volume metrics paired with margin metrics
- Acquisition metrics paired with retention metrics
- Cost metrics paired with capability metrics

### Step 8 — Cull aggressively

A typical organization arrives with 40+ tracked metrics. The final architected system should have:

- 1 north-star
- 3–5 lagging outcome KPIs
- 5–10 leading operational KPIs

That is 9–16 metrics total. Anything beyond this is operational reporting and should live in functional dashboards, not the strategic system.

## Hypotheses to Pressure-Test

1. **"The current KPI set produces motion but not progress."** Are people busy improving metrics that don't move the strategic outcome?
2. **"The lagging metrics are tracked but the leading metrics are not."** This is the most common pattern — and it makes intervention impossible.
3. **"The north-star is a vanity metric in disguise."** Does it capture value delivered, or activity performed?
4. **"At least one current KPI is being actively gamed."** Where would you game if you were optimizing for personal performance review?

## Quality Checks Before Sharing

- [ ] North-star metric defined and tests pass (moves with strategy, value-not-activity, measurable, ungameable)
- [ ] KPI tree decomposes the north-star MECE into operational components
- [ ] 3–5 lagging outcome KPIs selected, each tied to strategic outcome
- [ ] 5–10 leading operational KPIs identified, each with owner, cadence, formula
- [ ] Targets triangulated from history, benchmark, and strategic requirement
- [ ] Action thresholds (green / yellow / red / black swan) predefined
- [ ] Gaming test and proxy-failure test run on every metric
- [ ] Counterbalancing metrics paired where gaming risk is high
- [ ] Total system culled to 9–16 metrics

## Common Failure Modes

- **Reporting masquerading as management.** Tracking metrics that nobody acts on. Cut them.
- **All lagging, no leading.** A system that reports outcomes after they happen but cannot detect drift early.
- **Target inflation.** Setting easy targets to ensure green status. Or its inverse: setting impossible targets that the organization stops believing.
- **Metric proliferation.** Adding metrics every quarter without ever removing them. Architects subtract.
- **Decoupled ownership.** A metric without a single named owner is a metric nobody owns.
- **The dashboard fallacy.** Believing that displaying data is the same as managing performance. The dashboard is downstream of the thinking.

## Deliverable

A KPI tree decomposing the north-star, a defined metric set (1 north-star + 3–5 lagging + 5–10 leading), an owner / cadence / formula sheet for each metric, target tables with historical / benchmark / strategic anchors, and predefined action thresholds.
