<div align="center">

# 🎨 UX Builder

**An AI skill that applies 500+ empirically-validated UX principles — with real numbers, not opinions.**

[![Install](https://img.shields.io/badge/npx%20skills%20add-lgboim%2Fux--builder-4A90E2?style=for-the-badge&logo=npm)](https://skills.sh/lgboim/ux-builder)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![Works with Claude](https://img.shields.io/badge/Works%20with-Claude-blueviolet?style=for-the-badge)](https://claude.ai)

Works with **Claude · Cursor · Copilot · Gemini CLI · Cline · Codex · Amp** and more.

</div>

---

## What is this?

UX Builder is an installable AI skill that gives your agent deep, research-backed UX/UI expertise. Instead of vague advice like *"make it more intuitive"*, it gives you:

- **Specific rules** backed by Baymard Institute, Nielsen Norman Group, and WCAG 2.2
- **Exact numbers** — "top-aligned labels are 28% faster to scan than left-aligned"
- **Binary pass/fail verdicts** — 150+ checklist items with quantified business impact
- **Prioritized fixes** ranked by conversion or usability impact

This is the difference between a junior designer guessing and a senior UX researcher citing 200,000+ hours of usability studies.

---

## Install

```bash
npx skills add lgboim/ux-builder
```

That's it. Works globally with any supported AI agent.

---

## Quick Demo

After installing, just describe what you're building or paste a URL:

```
You: Audit my checkout flow — users are dropping off at step 2

Agent: ## UX Audit: Checkout Flow

### 🚨 Critical Issues (fix immediately)

**1. Forced account creation before purchase**
- Rule violated: Baymard Institute "Guest Checkout" guideline
- Impact: 28% of users abandon when forced to register
- Fix: Move account creation to the confirmation page, after purchase completes.
  Show "Save your details for next time?" as an optional step.

**2. Coupon field is prominently visible**
- Rule violated: Baymard coupon field placement research
- Impact: 27% of users who see it leave to search for discount codes and don't return
- Fix: Hide behind a "Have a promo code?" text link — collapsed by default.

**3. 6-step progress bar**
- Rule violated: Miller's Law + Baymard checkout length research
- Impact: Users perceive the process as too long; 18% abandon on sight
- Fix: Consolidate to ≤4 steps. "Shipping + Billing" can be one step.
```

---

## What It Covers

| Domain | What you get |
|--------|-------------|
| **UX Audits** | 150+ binary pass/fail rules, prioritized by business impact |
| **E-Commerce** | Checkout, cart, product pages, search, filters — Baymard-sourced |
| **Forms** | Field layout, validation timing, label alignment, input formatting |
| **Accessibility** | WCAG 2.2 AA compliance with exact thresholds (not approximations) |
| **Conversion Rate (CRO)** | A/B test findings with exact lift percentages |
| **Navigation & IA** | Desktop/mobile patterns, menu structures, hierarchy |
| **New Product Design** | Principle-backed decisions from first wireframe to launch |

---

## Example Prompts

These all work out of the box after installing:

```
"Audit this landing page: [URL or description]"
"Design a signup form following best practices"
"Is my navigation WCAG 2.2 AA compliant?"
"Why are users dropping off my product page?"
"What's the optimal checkout flow for mobile?"
"Review this component for accessibility issues"
"What are the most common UX mistakes in SaaS dashboards?"
```

---

## What's Inside

The skill bundles a structured knowledge base that gets loaded based on your question:

```
ux-builder/
├── SKILL.md                    ← Agent instructions
└── references/
    ├── foundations.md          ← Nielsen Norman heuristics, Fitts/Miller/Hick/Fogg laws, WCAG POUR
    ├── ecommerce.md            ← Baymard Institute e-commerce research (checkout, cart, search)
    ├── checklist.md            ← 150+ binary pass/fail audit rules
    └── metrics.md              ← Quantified thresholds, A/B data, business impact figures
```

The agent reads only the relevant files for your specific question — so responses stay fast and focused.

---

## Knowledge Sources

| Source | What it contributes |
|--------|-------------------|
| **Baymard Institute** | 200,000+ hours of e-commerce UX research, checkout/cart/form guidelines |
| **Nielsen Norman Group** | 10 Usability Heuristics, interaction design principles |
| **WCAG 2.2** | Accessibility compliance criteria (AA level) |
| **Fitts's Law** | Touch target sizing and placement |
| **Miller's Law** | Cognitive load, chunking, working memory limits |
| **Hick's Law** | Decision time vs. number of choices |
| **Fogg Behavior Model** | Motivation, ability, and prompts in UX |
| **ISO 9241-110** | Ergonomics of human-system interaction |

---

## Key Facts Worth Knowing

A sample of the data-backed rules this skill applies:

- Guest checkout visible by default → **28% fewer abandonments**
- Top-aligned form labels → **28% faster to complete** than left-aligned
- Single-column form layout → **15.4 seconds faster** than multi-column
- Hiding coupon field → eliminates **27% coupon-hunt abandonment**
- Progress bars with >4 steps → **increase** abandonment (not reduce it)
- Desktop hamburger menu → **~500% drop** in navigation engagement
- Inline validation (on blur) → **42% faster** form completion

---

## Compatible Agents

Installs as a universal skill. Tested with:

**Claude** · **Cursor** · **GitHub Copilot** · **Gemini CLI** · **Cline** · **OpenAI Codex** · **Amp** · **Zed AI** · **Continue**

---

## Contributing

Found a new empirical UX finding worth adding? PRs welcome.

The reference files are plain Markdown — easy to read and edit. Add findings to the appropriate file in `references/` with source and quantified impact.

---

## License

MIT © [lgboim](https://github.com/lgboim)
