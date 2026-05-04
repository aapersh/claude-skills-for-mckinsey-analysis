---
name: growth-barriers
description: Identify the real reason growth has stalled — not the symptom leadership is talking about. Use when revenue has plateaued, when growth is decelerating despite investment, or when the team is debating where to push next. Built around growth decomposition, constraint theory, and root-cause issue trees.
---

# Growth Barriers

## Purpose

Find the actual constraint holding growth back, distinguish it from its symptoms, and identify the highest-leverage intervention.

Growth problems are almost never what they look like on the surface. Sales blames marketing. Marketing blames product. Product blames sales. The senior associate's job is to break the circle.

## Governing Principle

**A system can only grow as fast as its tightest constraint allows. Find the constraint. Don't optimize anything else first.**

This is the Theory of Constraints applied to commercial growth: improvements anywhere except the bottleneck are illusions on the P&L.

## The Five Layers Where Growth Breaks

Growth breakdowns happen in one of five places. Diagnose in this order — do not skip ahead.

1. **Market layer** — is the addressable demand still growing, or has the market itself stalled?
2. **Acquisition layer** — can we still bring qualified prospects to the door at viable cost?
3. **Conversion layer** — do prospects become customers at the rate they used to?
4. **Expansion layer** — do customers grow in value over time the way the model assumed?
5. **Retention layer** — are we losing customers faster than we are replacing them?

The constraint is in exactly one of these layers — usually. Pretending it is in two simultaneously is how teams end up working on five things and fixing none.

## Workflow

### Step 1 — Decompose growth into its arithmetic components

Pull the last 8–12 quarters of data. Express growth as:

```
Revenue Growth = 
    (New customer revenue)
  + (Expansion revenue from existing customers)
  − (Churned revenue)
  − (Contraction from existing customers)
```

Then decompose each component:

- **New revenue** = leads × conversion rate × average deal size
- **Expansion** = % of base expanding × average expansion size
- **Churn** = % of base churning × average revenue per churn
- **Contraction** = % of base contracting × average reduction

Plot each line over time. The line that turned first is the suspect. The line that turned most is the constraint.

### Step 2 — Apply the "where did the slope change" test

For each component, identify the inflection point — the quarter where the trend visibly changed. Then ask:

- What changed in the business 1–2 quarters before that inflection? (The cause usually leads the effect.)
- What changed in the market in the same window?
- What changed inside the customer base (mix shift, segment movement)?

The inflection point dating is the most underused technique in growth diagnosis. Most teams describe what is happening now without anchoring when it started.

### Step 3 — Build the funnel waterfall (acquisition to revenue)

For new-customer growth specifically, build the full funnel with conversion rates at each stage:

```
Awareness  →  Lead  →  MQL  →  SQL  →  Opportunity  →  Closed Won  →  Activated  →  Retained
```

Calculate stage-to-stage conversion rates for the current period and 8 quarters ago. The stage with the largest absolute degradation is the bottleneck candidate.

Two diagnostic patterns:
- **Top-of-funnel collapse:** awareness or lead volume down → market or acquisition problem
- **Mid-funnel collapse:** lead-to-opportunity down → targeting or product-market-fit problem
- **Bottom-of-funnel collapse:** opportunity-to-close down → competitive, pricing, or sales execution problem

### Step 4 — Run the cohort analysis

For existing customers, plot revenue retention curves by cohort (by quarter of acquisition). Look for:

- **Are newer cohorts retaining worse than older ones?** → product or onboarding has degraded, OR customer mix has shifted to lower-quality segments
- **Are all cohorts decaying faster?** → market shift, competitive pressure, or pricing problem
- **Is expansion flattening across cohorts?** → upsell motion broken or product expansion ceiling hit

Cohort decay tells the truth that aggregate retention numbers hide.

### Step 5 — Build the issue tree for the suspect constraint

Once one layer is identified as the constraint, drill MECE into root cause:

```
Acquisition is the constraint
├── Volume problem
│   ├── Channel saturation (CAC rising in same channels)
│   ├── Channel decline (specific channels degrading)
│   └── Channel gap (new channels emerging we are not in)
├── Quality problem
│   ├── Targeting drift (reaching wrong audience)
│   ├── Message drift (positioning no longer resonates)
│   └── Offer drift (product or pricing no longer competitive)
└── Economics problem
    ├── CAC increasing faster than LTV
    ├── Payback period extending
    └── Mix shifting to lower-value segments
```

Every leaf must be testable with available data. If a leaf cannot be tested, it is a guess, not a hypothesis.

### Step 6 — Apply the "five whys" to the leaf

For the most likely leaf, ask why five times. The first three answers will be tactical. The fourth and fifth usually reveal the structural cause.

Example:
- *Why has the lead-to-opportunity conversion rate dropped?* → leads are lower quality
- *Why are leads lower quality?* → we are targeting a broader audience
- *Why are we targeting broader?* → we hit saturation in our core segment last year
- *Why didn't we expand into adjacent high-quality segments?* → our product positioning doesn't resonate there
- *Why doesn't it resonate?* → the product was built for a buyer profile that has matured out of the growth phase

The fifth answer is the strategic problem. The first four are symptoms.

### Step 7 — Size the prize and the cost

For the identified constraint, estimate:

- **Prize:** if we fully relieved this constraint, what is the incremental revenue / margin in 12 and 24 months?
- **Cost:** what investment, capability, or time is required?
- **Confidence:** what is the probability of success based on evidence?

Expected value = Prize × Confidence − Cost. If this is negative, the constraint may not be the right one to attack — or the strategy needs reframing rather than fixing.

## Hypotheses to Pressure-Test

1. **"The constraint leadership is focused on is not the actual constraint."** Where is the team's attention vs. where is the data pointing?
2. **"The growth problem is a mix problem, not a volume problem."** Is the business growing in the wrong segments and contracting in the right ones?
3. **"The ICP has aged."** Is the buyer profile that drove early growth now structurally smaller, less profitable, or harder to reach?
4. **"The growth playbook that worked at $10M is failing at $100M."** Has the business outgrown the motion that built it?

## Quality Checks Before Sharing

- [ ] Growth decomposed arithmetically into new / expansion / churn / contraction
- [ ] Inflection point dated for each component
- [ ] Full funnel waterfall built with stage conversion rates, then vs. now
- [ ] Cohort analysis shows retention curves by acquisition quarter
- [ ] Single constraint identified — not "we have many problems"
- [ ] Issue tree on the constraint is MECE and every leaf is data-testable
- [ ] Five-whys traced to a structural cause, not a tactical one
- [ ] Expected value calculated for relieving the constraint

## Common Failure Modes

- **Treating multiple symptoms as multiple problems.** Five symptoms usually trace to one cause. Find the cause.
- **Boiling the ocean.** Working on every funnel stage simultaneously. Constraint theory says this destroys value.
- **Mistaking a comp problem for a growth problem.** Sometimes the issue is sales incentives, not strategy. Diagnose accordingly.
- **Optimizing yesterday's funnel.** The growth motion that got the company here is rarely the one to take it to the next phase.
- **Survivor bias on cohorts.** Looking only at retained customers and missing the ones who churned silently.

## Deliverable

A growth decomposition chart (8–12 quarters), a funnel waterfall comparing current vs. baseline period, a cohort retention chart, an issue tree on the identified constraint, and a one-page recommendation with prize / cost / confidence sized.
