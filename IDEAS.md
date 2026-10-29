# Idea menu - full-stack developer / UI / writing (DRAFTS)
Rewrite each in your own words before submitting (handbook: no pasted AI text). Prepare inputs beforehand (self-made, synthetic, Gemini-prepared, or verified CC0 / permissively licensed public GitHub). No AI tools or AI editor features on camera. Target recording 25-40 min incl. intro and 3-4 min epilogue. Coding tasks may type up to 35%, in segments under 45 s. Check each app against the banned list first.

Format: Domain/Role | Goal | Starting materials | Steps (app per step) | Deliverable

## 1. Fix a failing API endpoint (Express) - VS Code, Chrome DevTools, Terminal
- Role: Full-stack developer on a small SaaS team
- Goal: A support lead needs a bug fixed where the /orders endpoint returns wrong totals when a discount code is applied; I will reproduce, find the root cause, patch it, and prove the fix with passing tests.
- Starting: Small Node/Express project with a seeded bug and 6 unit tests, written before recording (synthetic, MIT).
- Steps: Terminal - run tests, show failures; Chrome (DevTools Network) - reproduce via the demo page and inspect the bad response; VS Code - trace the discount logic, fix rounding/order-of-operations bug; Terminal - rerun tests, add one regression test; VS Code - commit message.
- Deliverable: patched orders.js, new regression test, test output screenshot (final output 1-3).

## 2. Responsive + accessibility fix of a landing page - VS Code, Chrome (DevTools + Lighthouse), Google Sheets
- Role: Front-end developer / UI designer
- Goal: A marketing manager needs a landing page that works on mobile and meets basic WCAG AA; I will audit it, fix the worst issues, and show the Lighthouse scores improve.
- Starting: Self-built static HTML/CSS page with seeded issues (fixed-width hero, low-contrast button, missing alt text, no focus styles).
- Steps: Chrome - run Lighthouse and device-mode checks; Google Sheets - log each issue with WCAG criterion and severity; VS Code - fix CSS/HTML; Chrome - rerun Lighthouse and verify at 3 breakpoints.
- Deliverable: fixed index.html + styles.css, issue log (.xlsx), before/after Lighthouse screenshots.

## 3. Slow query diagnosis and indexing - DBeaver, Google Sheets, VS Code
- Role: Backend developer / database engineer
- Goal: An ops manager needs the monthly sales report query to run in seconds instead of minutes; I will measure, add the right indexes, and document the speedup.
- Starting: Synthetic SQLite database (~200k rows, customers/orders/items) generated before recording.
- Steps: DBeaver - run the slow query, read EXPLAIN QUERY PLAN; VS Code - write index migration script; DBeaver - apply it, rerun and compare; Google Sheets - results table (before/after timings, plan changes) and a recommendation.
- Deliverable: migration.sql, timing comparison sheet (.xlsx), optimized query file.

## 4. Backlog prioritisation and sprint plan - Linear/Jira/Trello (pick one), Google Sheets, Word/Google Docs
- Role: Technical project manager / lead developer
- Goal: A product owner needs a two-week sprint plan from a 25-item backlog with a capacity of 4 developers; I will score items, resolve dependencies and produce a committed sprint with risks.
- Starting: Synthetic backlog (titles, estimates, dependencies, business value) in a CSV prepared before recording.
- Steps: Google Sheets - import and score (value/effort, dependency flags), compute capacity; PM tool - create the sprint board with the selected tickets; Word/Docs - one-page sprint brief with scope, risks, what was deferred and why.
- Deliverable: scoring sheet (.xlsx), board export/screenshot, sprint brief (.docx). Low typing, mostly mouse - good fit.

## 5. Merge-conflict resolution and code review - GitHub (Chrome), VS Code, Terminal
- Role: Senior developer
- Goal: A team lead needs two feature branches merged safely; I will review the pull request, resolve conflicts keeping both features working, and leave review notes.
- Starting: Small public-domain/MIT demo repo prepared with two conflicting branches.
- Steps: Chrome (GitHub) - review PR diff, comment on 3 issues; VS Code - resolve conflicts; Terminal - run tests, complete merge; Chrome - post summary.
- Deliverable: resolved branch (zipped repo), review comments (screenshot/export), test results.

## 6. API documentation + README - VS Code, Chrome (Swagger UI), Word/Google Docs
- Role: Developer / technical writer
- Goal: New hires need accurate API docs; I will inspect a small API, verify each endpoint in Swagger UI, and write a README and endpoint reference.
- Starting: Small API with OpenAPI spec prepared before recording.
- Steps: Chrome (Swagger UI) - call endpoints, record real responses; VS Code - write README sections and fix spec mistakes; Docs/Word - formatted endpoint reference with examples.
- Deliverable: README.md, corrected openapi.yaml, endpoint reference (.docx/.pdf). Writing tasks allow 35% typing.

## 7. SwiftUI layout bug (Dynamic Type + dark mode) - Xcode (+ Simulator), Preview
- Role: iOS developer
- Goal: A product designer needs a profile screen that stays readable at large text sizes and in dark mode; I will find and fix the layout/contrast bugs and verify in the Simulator.
- Starting: Small SwiftUI project with seeded layout issues.
- Steps: Xcode - run in Simulator at large Dynamic Type and dark mode, capture failing screens; Xcode - fix views (layout, colours); Simulator - verify; Preview - annotate before/after screenshots.
- Deliverable: Xcode project zip, before/after annotated PDF. Risk: heavy on resources - do a test recording.

## 8. (Only if you own Sketch/Affinity Designer/Canva) UI kit to code handoff
- Role: UI designer/developer. Design a small component set, export assets and specs, implement in VS Code, check in Chrome. Needs a design app that is NOT on the banned list (Figma, Penpot are banned).
