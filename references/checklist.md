# Complete UX/UI Binary Audit Checklist
## 150+ Pass/Fail Items — Use for Comprehensive UX Audits

This checklist covers every binary rule in the master database. Use it when performing a full UX audit. Mark each item: ✅ Pass | ❌ Fail | N/A (not applicable)

---

## GUEST CHECKOUT & ACCOUNT

- [ ] Guest checkout is available
- [ ] Guest checkout is the most prominent, default option
- [ ] Account creation is delayed until AFTER purchase completes
- [ ] Guest checkout option is visible even for returning/logged-in users
- [ ] No forced registration before checkout begins

---

## FORM FIELD OPTIMIZATION

- [ ] Single "Full Name" field used (not split First/Last)
- [ ] Address Line 2 is hidden behind "Add Apt. #, Suite, Floor" link
- [ ] Billing address defaults to "Billing = Shipping" with option to change
- [ ] Coupon code field is hidden behind "Got a promo code?" text link
- [ ] Credit card number auto-formats (4-4-4-4 groups)
- [ ] Security code (CVV) has visual thumbnail showing its location on card
- [ ] Guest checkout has ≤8 visible fields total
- [ ] All form field labels are top-aligned (not left-aligned)
- [ ] No "Reset" button exists (or if required, is ≥200px from "Submit")
- [ ] No "Clear Form" button exists

---

## VALIDATION & ERROR HANDLING

- [ ] Inline validation triggers on blur (when user leaves field), NOT while typing
- [ ] Error messages disappear per-keystroke as user corrects input
- [ ] All errors are shown simultaneously (not just the first error)
- [ ] Errors are displayed adjacent to the offending field
- [ ] Errors are programmatically associated via aria-describedby
- [ ] All error inputs have aria-invalid="true"
- [ ] Error messages are in plain language (no error codes like "Error 0x442")
- [ ] Error messages suggest a specific solution ("Include an @ symbol")
- [ ] Green checkmarks confirm successful field validation
- [ ] Luhn algorithm validates credit card numbers in real-time

---

## INPUT MASKING & FORMATTING

- [ ] Phone numbers auto-format as user types
- [ ] Dates auto-format (MM/DD/YYYY or regional standard)
- [ ] Credit card numbers auto-format (4-4-4-4)
- [ ] SSN auto-formats (XXX-XX-XXXX) where applicable
- [ ] Email fields have autocapitalization disabled on mobile
- [ ] Password fields have visibility toggle (eye icon) on mobile
- [ ] Invalid characters blocked in real-time for numeric-only fields

---

## INPUT CONTROL TYPES

- [ ] Radio buttons used for ≤5 mutually exclusive options (not dropdowns)
- [ ] Quantity selection uses +/- buttons AND text input (not dropdown only)
- [ ] Price/numeric range filters allow open input or slider (not fixed brackets)

---

## CART & CHECKOUT INTERACTION

- [ ] Cart icon badge shows item count
- [ ] Cart icon badge shows subtotal
- [ ] "Add to cart" confirmation uses persistent overlay (not transient/fading)
- [ ] Form changes auto-persist on blur/change (no "Apply" or "Update" buttons)
- [ ] Checkout progress indicator shows ≤4 steps (or multi-step wizard for 5+ steps)
- [ ] Multi-step forms begin with lowest-friction questions
- [ ] Each step validates before allowing progression to next step
- [ ] Progress shows initial state "completed" to trigger Endowed Progress Effect

---

## PRODUCT DETAIL PAGE (PDP)

- [ ] Product information shown in vertical sections/accordions (not horizontal tabs)
- [ ] In-scale images provided (product shown next to human or known object)
- [ ] Wearables shown on human models (not mannequins or cut-outs)
- [ ] Gallery navigation uses thumbnails (not dots)
- [ ] Gallery thumbnails not truncated
- [ ] ≥3 product images provided (target: 5–15 for visual products)
- [ ] Unit pricing displayed for bulk/multi-quantity items
- [ ] Unit price and total price displayed at different font sizes
- [ ] Sold-out variants shown with clear "Sold Out" visual tag
- [ ] Price is prominent and clearly visible

---

## PRODUCT LISTING PAGE (PLP)

- [ ] Color/style variations combined into one listing with swatches (not duplicate listings)
- [ ] Sold-out items shown alongside available items (not hidden)
- [ ] Default sort is "Relevance" or "Best Sellers" (not Alphabetical A-Z)
- [ ] Same-type filters use OR logic (selecting Blue + Black shows items that are Blue OR Black)
- [ ] "View All" option available at each category/subcategory level
- [ ] At least 3 product thumbnails visible from listing without leaving page

---

## NAVIGATION

- [ ] Desktop uses fully visible navigation (no hamburger menu)
- [ ] Mega-menus have 200–300ms hover delay (prevents accidental activation)
- [ ] Current page/section is highlighted in navigation
- [ ] Breadcrumbs are displayed to show hierarchy location
- [ ] Navigation follows platform conventions (cart icon top-right, search top-right/center)

---

## SEARCH

- [ ] Search bar located in upper-right or top-center
- [ ] Search field is open/visible (not icon-only)
- [ ] Autocomplete suggestions appear after 2–3 characters
- [ ] Autocomplete is typo-tolerant
- [ ] Autocomplete supports abbreviation mapping ("3pc" → "3-piece", "13 in" → "13 inch")
- [ ] Autocomplete includes category scope (e.g., "Nike" in Shoes, Nike in Clothing)
- [ ] Autocomplete shows 5–8 suggestions maximum (no internal scrollbar)
- [ ] Zero-results state provides "Clear Search" or "Browse Categories" escape
- [ ] No redundant data entry in search or filter flows

---

## ACCESSIBILITY — CONTRAST

- [ ] Body text has ≥4.5:1 contrast ratio (no rounding; 4.499:1 is a FAIL)
- [ ] Large text (18pt+ or 14pt bold+) has ≥3:1 contrast ratio
- [ ] UI components (buttons, input borders, icons) have ≥3:1 contrast ratio
- [ ] Focus indicators have ≥3:1 contrast ratio
- [ ] No contrast values have been rounded to meet thresholds

---

## ACCESSIBILITY — TOUCH TARGETS

- [ ] All touch targets are ≥44×44 CSS pixels (≥48×48 dp preferred for cross-platform)
- [ ] Minimum 8px dead space between adjacent touch targets
- [ ] Small target error rates are not elevated (verify with user testing if possible)

---

## ACCESSIBILITY — KEYBOARD & FOCUS

- [ ] All functionality is operable via keyboard only
- [ ] Tab order is logical and follows reading order
- [ ] All interactive elements have visible focus indicators
- [ ] Focus indicators are never obscured by other content
- [ ] Sticky headers never obscure the focused element during keyboard nav
- [ ] When modal opens, focus moves to first interactive element inside it
- [ ] Tab focus cannot escape to background content when modal is open
- [ ] Pressing Escape closes modal and returns focus to trigger element

---

## ACCESSIBILITY — ALT TEXT & ARIA

- [ ] All meaningful images have alt text (≤150 characters)
- [ ] Alt text does NOT include "image of" or "photo of" prefix
- [ ] Decorative images have alt="" (empty alt attribute)
- [ ] All form inputs are associated with <label> elements
- [ ] Error inputs use aria-invalid="true" paired with aria-describedby
- [ ] Semantic HTML used throughout (nav, main, article, section, header, footer)

---

## ACCESSIBILITY — MOBILE & MOTION

- [ ] App does NOT lock to Portrait or Landscape orientation only
- [ ] Layout remains usable at 1.6× zoom without horizontal scroll
- [ ] Sticky headers are partially persistent on mobile (<20% viewport height)
- [ ] Infinitely looping background videos have physical pause button OR auto-stop after 5 seconds
- [ ] Animations respect CSS prefers-reduced-motion: reduce media query
- [ ] Font size minimum 16px for body text (no zooming required to read)

---

## PERFORMANCE & FEEDBACK

- [ ] Page load time ≤1 second (or ≤3 seconds with loading indicator shown)
- [ ] Loading indicators displayed for all operations taking >1 second
- [ ] Images are optimized for fast delivery
- [ ] No unnecessary blocking JavaScript
- [ ] Operations perceived as "instant" (<0.1 seconds) have no spinner
- [ ] Operations >1 second always show progress (spinner, bar, or status message)

---

## GENERAL UX PRINCIPLES

- [ ] Single-column form layout used (not multi-column)
- [ ] Information grouped into ≤9 items (Miller's Law)
- [ ] Easy/low-friction questions come before high-friction ones (Commitment & Consistency)
- [ ] Options visible without requiring memory (Recognition over Recall)
- [ ] Platform conventions and industry standards followed (Jakob's Law)
- [ ] Irrelevant information removed from checkout/key flows (Aesthetic & Minimalist Design)
- [ ] Users can always undo or cancel key actions (User Control & Freedom)
- [ ] System provides appropriate feedback within reasonable time (Visibility of System Status)
- [ ] Descriptions are specific, not generic (e.g., "Very good breakfast" not "Breakfast included")
- [ ] Desktop hamburger menus are absent
- [ ] Specific small details included in product/service descriptions (increase confidence)
