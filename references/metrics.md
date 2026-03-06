# UX Quantified Metrics & Business Impact Reference
## Every Specific Number, Threshold, and Measured Finding

Use this file when justifying recommendations with data, estimating impact, or citing specific research findings.

---

## CONVERSION & BUSINESS IMPACT

| Metric | Value | Source / Context |
|--------|-------|-----------------|
| Overall checkout conversion lift (all 32 heuristics) | **+35.2%** | Baymard Institute aggregate |
| Average cart abandonment rate | **70.19%** | Industry average |
| Abandonment due to complex/long checkout | **18–26%** | Of total abandonment |
| Expedia Company Field removal | **+$12M annual profit** | Single field removal case study |
| Multi-step form conversion lift | **11% → 46%** | Venture Harbour case study |
| Multi-step forms w/ low-friction start | **53% conversion rate** | Baymard finding |
| TRNN (intent-trained recommendations) | **+7.34% Purchase-Through Rate** | ML recommendation research |
| Multi-Armed Bandit algorithm CTR | **+6.13% CTR** | Batch-updated MAB |
| Multi-Armed Bandit algorithm CVR | **+16.1% conversion rate** | Batch-updated MAB |
| Showing sold-out items (Booking.com) | Increases overall bookings | Paradoxical scarcity validation |
| WCAG-compliant navigation | **+24% task completion rate** | Accessibility impact |

---

## FORM PERFORMANCE METRICS

| Metric | Value | Context |
|--------|-------|---------|
| Inline validation — task success rate | **+22%** | vs. no inline validation |
| Inline validation — error rate | **-22%** | vs. no inline validation |
| Inline validation — completion time | **-42%** | vs. no inline validation |
| Inline validation — user satisfaction | **+31%** | vs. no inline validation |
| Single-column layout speed advantage | **15.4 seconds faster** | vs. multi-column |
| Top-aligned labels speed advantage | **28% faster to process** | vs. left-aligned labels |
| Radio buttons speed advantage (≤5 options) | **2.5 seconds faster** | vs. dropdown |
| Multi-step form trigger threshold | **>7 visible fields** | Best practice |
| Optimized checkout field count | **6–8 fields** | vs. average 11.3–12.8 |
| Field reduction potential | **20–60%** | Most checkout forms |

---

## CHECKOUT FIELD FRICTION POINTS (FAILURE RATES)

| Field / Feature | Failure Metric |
|----------------|----------------|
| Address Line 2 visible by default | **30% of users pause/question** |
| Full Name (split First/Last) | **42% of users type full name in First box** |
| Full Name (single field) | Only **4% of users hesitate** |
| Sites using split First/Last (incorrect) | **89% of sites** |
| Billing address forced when same as shipping | **24% of sites** |
| Prominent coupon field visible | **35% of sites** (triggers off-site abandonment) |
| CVV without visual hint | **38% of users pause** |
| Account creation forced at checkout | **84% of sites fail** |
| Guest checkout not prominent enough | **47% of sites** |
| Address Line 2 shown by default | **75% of sites fail** |
| Credit card no auto-formatting | **15% of sites fail** |
| Quantity dropdown-only | **61% of sites fail** |
| "Apply" button unnecessary | **22% of sites include it** |

---

## PRODUCT PAGE METRICS

| Metric | Value |
|--------|-------|
| Users judging product size from images | **42%** |
| Sites failing to provide in-scale images | **91%** |
| Sites failing to show wearables on models | **55%** |
| Information missed in horizontal tabs | **27% miss rate** |
| Information missed in vertical sections | **8% miss rate** |
| Improvement from tabs → vertical sections | **19 percentage points** |
| Sites providing too few images | **80%** |
| Sites failing unit pricing | **74%** |
| Color variation failure (duplicate listings) | **42% of sites** |
| Images missed with dots nav/truncated thumbs | **50–80%** |
| Minimum images for visual products | **3–15 images** |

---

## NAVIGATION & SEARCH METRICS

| Metric | Value |
|--------|-------|
| Desktop hamburger menu engagement reduction | **~500% less engagement** |
| Mobile sites missing current location highlight | **95% fail** |
| Mobile sites missing "View All" | **42% fail** |
| Search category scope failure (mobile) | **77% fail** |
| Search abbreviation mapping failure (mobile) | **58% fail** |
| Autocomplete trigger threshold | **2–3 characters** |
| Autocomplete max suggestions | **5–8 (no scrollbar)** |
| Filtering OR logic failure rate | **15% of sites** |
| Sticky header navigation time savings (desktop) | **~22%** |

---

## PERFORMANCE / PAGE LOAD METRICS

| Load Time | Approximate Bounce Rate |
|-----------|------------------------|
| 1 second | **~20% bounce rate** |
| 3 seconds | **~40% bounce rate** |
| 5 seconds | **~60% bounce rate** |
| 10 seconds | **>90% bounce rate** |
| 1s → 10s increase | **+123% bounce probability** |
| "Instant" perception threshold | **0.1 seconds** |
| "Seamless" perception threshold | **1.0 second** |
| Spinner required above | **>1.0 second** |

---

## ACCESSIBILITY THRESHOLDS

| Requirement | Threshold |
|-------------|-----------|
| Body text contrast (AA) | **4.5:1 minimum** (no rounding) |
| Body text contrast (AAA) | **7:1 minimum** |
| Large text contrast (AA) | **3:1 minimum** |
| Large text contrast (AAA) | **4.5:1 minimum** |
| UI components / buttons contrast | **3:1 minimum** |
| Touch target size (WCAG AA) | **24×24 CSS px minimum** |
| Touch target size (WCAG AAA) | **44×44 CSS px recommended** |
| Touch target size (Android) | **48×48 dp** |
| Touch target size (iOS) | **44×44 pt** |
| Cross-platform safe minimum | **48×48** |
| Touch target spacing | **8px dead space minimum** |
| Small target error rate increase | **+30% errors** |
| Motor impairment target | **18mm** |
| ASD user target | **57px** |
| Blind user target | **10–15mm** |
| Alt text maximum length | **150 characters** |
| Mobile sticky header max height | **20% of viewport** |
| Zoom support | **1.6× pinch without horizontal scroll** |
| Minimum readable font size | **16px** |
| Mega-menu hover delay | **200–300ms** |
| Looping video auto-stop threshold | **5 seconds** |

---

## BAYMARD RESEARCH SCALE

| Research Scale | Value |
|----------------|-------|
| Total research hours (primary claim) | 200,000+ hours |
| Total test sessions | 4,400+ |
| Verified guidelines count | 771 (tiered, evolving database) |
| Automated audit accuracy | **95%** (vs. 20–75% for generic AI) |
| Checkout research scope | Large-scale e-commerce |

---

## DOCUMENTED CONTRADICTIONS (USE WHEN RELEVANT)

| Conflict | Resolution |
|----------|-----------|
| 35.2% conversion lift = aggregate, not single change | Combine all 32 heuristics for maximum impact |
| Progress bars reduce AND increase abandonment | Keep steps ≤4 max; use wizard for 5+ |
| Full Name single field vs. marketing tool compatibility | UX wins → add backend data transformation |
| Browser validation (stops at first error) vs. best practice (show all errors) | Implement custom JS validation to show all simultaneously |
| Reset buttons: user need vs. UX anti-pattern | Replace with "Start Over" text link + confirmation |
| Fitts's Law applicability to touchscreens | Use as guideline; finger occlusion is a real factor |
| WCAG (44px) vs. Android (48dp) vs. ergonomic (35–40px) | Use 48×48 for maximum cross-platform safety |
