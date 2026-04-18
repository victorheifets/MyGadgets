# Domain Add-On Questions

Append these after base questions in Phase 1. Pick the block matching the classified domain.

---

## Food / IoT / Hardware
```
7. How will this be viewed? (phone held in hand, wall tablet, desktop browser)
8. How many probes / devices at once? (1, 2–4, 5+)
9. Audio alerts for key events? Yes / No / Nice to have
10. Real-time data from hardware, or reference/calculator UI?
11. Show visual doneness/status reference? Yes / No
```

## HR / Compliance / Legal
```
7. How many workflow steps? (single form, multi-step wizard, dashboard with list)
8. Role-based access? (manager approves, employee submits, admin sees all)
9. Deadlines or time-sensitive states to surface?
```

## Finance / Analytics
```
7. Typical data volume? (rows per table, number of charts)
8. Primary time ranges? (daily, weekly, monthly, custom)
9. Export or download needed?
```

## Healthcare
```
7. Patient-facing or clinician-facing?
8. Sensitive data visible on screen?
9. Critical alerts that need to interrupt the user?
```

## Developer Tools
```
7. Terminal-style or GUI?
8. Live/streaming data or static snapshots?
9. Keyboard-first or mouse-first?
```

## SaaS / Internal Tools
```
7. End customers, internal ops team, or admins?
8. Multi-tenant (data scoped per org) or single org?
9. Permission levels or roles that affect what's visible?
```

## Consumer / Lifestyle
```
7. Used daily (habit) or occasionally (reference)?
8. Gamification or progress elements needed?
9. Social / sharing features?
```

## E-commerce / Catalog
```
7. How many products in a typical view? (handful, dozens, hundreds)
8. Cart and checkout needed, or catalog-only?
9. Trust signals needed? (reviews, badges, guarantees)
```

## Education / Learning
```
7. Student-facing or instructor-facing?
8. Progress/completion tracking central to the UI?
9. Timed elements? (deadlines, quizzes, countdowns)
```

## Marketing / Content
```
7. Single user or team creates content?
8. Approval or publishing workflow visible?
9. Performance data (clicks, conversions) shown alongside content?
```

## Travel / Transportation
```
7. What booking variants or configurations exist? (affects whether form is simple or branching)
8. What participant types or categories exist, and do they have different rules or pricing?
9. Fixed dates or flexible? (affects date-flexibility UI)
10. Selection step needed before confirmation? (e.g., specific slot, option, upgrade)
11. Loyalty program, points balance, or member status visible?
```

---

## File Import / Upload Add-On
If the request involves file import, upload, or bulk data ingestion (any domain), also add:
```
I. What file formats accepted? (CSV, XLSX, both?)
II. Always a header row, or might some files start with data on row 1?
```

---

## Multi-Step Flow Gate (S1–S5)
If the request involves a wizard, booking flow, multi-screen checkout, or onboarding — these are MANDATORY even if the user says "just build it". A complex flow cannot be built correctly without this spec:
```
S1. What are ALL the steps? (list every screen the user touches)
S2. What data carries forward between steps?
S3. What entity types or variants exist that affect what the user sees? (e.g., subscription tier vs one-time, individual vs group, item category, user role)
S4. Can the user go back? (back button on every step, or just abandon?)
S5. What are the confirmation + success states?
```
