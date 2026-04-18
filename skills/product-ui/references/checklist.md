# Pre-Delivery Checklist

Run this before Phase 4. Fix failures inline — do not deliver until all items pass.

---

## Aesthetic
- [ ] Visual world is felt throughout — fonts, spacing, shadows, backgrounds, motion
- [ ] No generic fonts (Inter, Roboto, Arial, Space Grotesk) used as display fonts
- [ ] Dominant color + sharp accent principle applied
- [ ] Unforgettable element is the visual hero
- [ ] Complexity matches aesthetic vision (expressive = elaborate, functional = precise)

## Visual Quality
- [ ] No emojis used as icons — SVG only (Heroicons/Lucide)
- [ ] All icons from a consistent icon set
- [ ] Hover states don't cause layout shift
- [ ] Atmosphere/background appropriate to visual world

## Interaction
- [ ] All clickable elements have `cursor-pointer`
- [ ] Touch targets ≥ 44×44px
- [ ] Hover states provide clear visual feedback
- [ ] Transitions are smooth (150–300ms)
- [ ] Focus states visible for keyboard navigation
- [ ] `prefers-reduced-motion` respected

## Contrast & Visibility

**Light mode:**
- [ ] Body text: minimum `#0F172A` — never lighter than a mid-gray
- [ ] Translucent/glass surfaces: opacity not below 80% — must remain legible against background
- [ ] Borders: visibly distinct from the background — never near-invisible

**Dark mode:**
- [ ] Body text: minimum `#E2E8F0` — never darker than a mid-gray
- [ ] Borders: visibly distinct from the dark background — never near-invisible
- [ ] Icons/SVGs visible against dark backgrounds

**Both modes:**
- [ ] Minimum contrast ratio 4.5:1 for normal text
- [ ] Status colors (success/warning/error) distinguishable without color alone

## Layout
- [ ] Floating navbars have `top-4 left-4 right-4` offset
- [ ] Fixed navbars: content doesn't hide beneath them
- [ ] Consistent max-width across all pages
- [ ] No horizontal scroll on mobile
- [ ] Responsive at 375px, 768px, 1024px, 1440px

## Accessibility
- [ ] All images have alt text
- [ ] Form inputs have labels
- [ ] `aria-label` on icon-only buttons
- [ ] Color is not the only indicator
- [ ] Tab order matches visual order

## States
- [ ] All states from Phase 2d are implemented and reachable
- [ ] Empty state has a CTA (not just "No data")
- [ ] Loading state shown for any async >300ms
- [ ] Error state has a recovery path

## Visual Verification
- [ ] Playwright screenshot taken (desktop) — or noted as skipped with reason
- [ ] Playwright screenshot taken (375px mobile) — or noted as skipped with reason
- [ ] No visual issues found in screenshots (overflow, contrast, broken layout)

## Self-Review Lens (run last, silently)

For each thing that looks off: *"Would a real user dislike this, and why?"*
Then: *"Is the likelihood of fixing it above 50%?"*
- Yes → fix it before delivering. Don't mention it.
- No → flag it to the user with the reason it wasn't fixed.
