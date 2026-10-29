# Plan: Responsive-layout diagnosis (Chrome DevTools + Word)  ~25 min recording

## Why this idea works
Maven draft (Oct 29): diagnose ONE responsive problem, compare two widths in DevTools, test a CSS fix visually, document before/after in Word. 2 apps, both unrestricted. Mostly mouse-driven; low typing risk. Handbook: judgment + checked result, not app navigation.
Risk: generic. Make it specific (below) so the Idea Check's uniqueness test passes.

## Sharper version (REWRITE IN YOUR OWN WORDS before submitting)
- Domain / Role: Full-stack developer doing UI quality assurance for a SaaS company
- Goal: The developer maintaining a pricing page needs to know why the plan-comparison table breaks on phones and which fix to ship; I will diagnose the overflow at phone width, test two CSS fixes in DevTools, recommend one, and verify it at three widths.
- Starting materials: A small self-made pricing page for a fictional product (HTML/CSS, synthetic content, no external images or fonts). Inspection, diagnosis and recommendation are left for the recording.
- Steps: 1) Chrome DevTools - compare 1280px and 375px, find the element causing horizontal overflow, read box model/computed styles. 2) Chrome DevTools - live-test fix A (scrollable wrapper) and fix B (stacked layout), note effects on readability and tap targets. 3) Word - build the recommendation: before/after screenshots, chosen fix and why, CSS snippet. 4) Chrome DevTools - verify the chosen fix at 375, 768 and 1280px; Word - record the verification.
- Deliverable: Responsive-layout-recommendation.docx (a reviewer can check it contains before/after screenshots, the chosen fix, the CSS and a 3-width verification table).
- Apps: Google Chrome, Microsoft Word. (Safari/Chrome are allowed; Word is allowed.)

## Materials (do BEFORE recording)
1. Create the page. Either hand-write it, or use Gemini (only allowed AI, only before recording; then write "AI-generated before recording" in Final Notes). Gemini prompt:
   "Write a single-file HTML+CSS pricing page for a fictional analytics tool called 'Lumen'. Include a header with nav, a hero, and a 4-column plan comparison table (Free/Pro/Team/Enterprise, 8 feature rows). Use only system fonts, no images, no external links or CDNs. Deliberately make the table cause horizontal page overflow below 600px (fixed column widths totalling about 900px) and give the nav links small tap targets. Fictional content only. Do not add comments explaining the bugs."
2. Open it in Chrome once to confirm the bug at 375px. Save as `input 1.html`.
3. Check: no real names/brands/logos, no watermarks, no personal info in the file or path.

## Setup (once)  [handbook "Getting Set Up" and "Desktop Setup"]
Okta/Studio access, Insightful (SSO, Odin timer), TaskRecorder 2.4.4 (Apple silicon dmg), Xcode + Accessibility Inspector running (window closed via red button, not quit), clock seconds ON, Dock left/right + not auto-hidden, English, empty Desktop, built-in wallpaper, Do Not Disturb, fresh Chrome profile (no sign-in, no import), Mac renamed, Word signed in with mercor.expert/anonymised account or signed out, no profile photo. Change a UI element each recording (e.g. dark mode, Dock size). Test recording: check audio, >0.5 screenshots/second, Accessibility Inspector running.

## Order of work and timer
1. Finalise idea text -> submit in Studio (Odin Production Full Workflow > + Create Task). Wait for "Idea Approved". (Timer OFF while waiting.)
2. Build and test the page; rehearse twice (aloud, no recording, or test recording).
3. Studio tech setup checklist -> "Idea Approved: Start Recording".
4. Prepare: Goal doc in Word (ONLY the approved Goal, nothing else; not Notes/TextEdit), paste Goal + app list into TaskRecorder, draft Metadata.rtf (Request = Goal; Task Description = numbered steps; Topology filled in after recording).
5. Record (timer ON). 6. Validate, package, upload, AutoQC, submit.

## Run of show (target 22-28 min incl. 3-4 min epilogue)
0:00 Start Recording, minimize TaskRecorder. Say exactly: "I will be beginning my task soon. Here is the workflow I have in mind." (<20 s). Minimize the Goal doc.
0:20 Chrome: open input 1.html. Narrate: what the page is, who the reader is. Open DevTools (View > Developer > Developer Tools), toggle device toolbar. [announce any shortcut]
2:00 Compare 1280 vs 375: show horizontal scrollbar/overflow. Find the culprit via Elements panel (hover to highlight, check width). Read Computed/box model values aloud.
7:00 Test fix A (wrapper with overflow-x:auto) in the Styles pane; judge readability and sticky first column; capture screenshot (right-click node > Capture node screenshot).
11:00 Revert, test fix B (stack cells as cards at <600px); judge tap targets (>=44px) and scanning of plan features.
15:00 Decide: choose one fix; say why (user impact, maintenance cost, accessibility). Capture after screenshot.
16:00 Word: new document, title, headings; insert before/after screenshots (Insert > Pictures); short typed sections (<45 s each); CSS snippet (typed or pre-written in Word? - prepared snippets pasted from a file are fine).
21:00 Chrome: verify chosen fix at 375, 768, 1280; Word: add small verification table (width, overflow? Y/N, tap targets OK?).
23:30 Save in Word. Epilogue (3-4 min, mouse can be still): outcome and verification, why that fix, a problem hit and how solved, limits (one page, one browser, no real-device test), what you'd do next.
STOP: bring TaskRecorder forward, Stop Recording, wait for Idle.

Rules to keep in mind while recording: narrate What + Where + Why for each action; no vague "this/here"; announce shortcuts; pause ~1 s after clicks; no silence >45 s; typing <=25% total; keep menu bar, clock, Dock visible; no full screen; one clear window or side by side; no Slack/Studio/Insightful on screen; no AI features (turn off DevTools AI assistance). At least one final output (the .docx) is created ON camera.

## Packaging
Deliverables.zip: `input 1.html`, `artifact 1.png` (before), `artifact 2.png` (fix A attempt), `artifact 3.png` (after), `final output 1.docx` (rename the Word file when you zip - the AutoQC naming check requires "final output N"). Separately upload video.mp4, the original recording_TIMESTAMP.zip, Metadata.rtf.
Final Notes: "input 1: AI-generated before recording" (if Gemini) or "written by me".
Metadata.rtf Topology example (must match what you actually do): Chrome - LOOKUP; Chrome - MODIFY; Word - CREATE; Chrome - LOOKUP; Word - MODIFY.
