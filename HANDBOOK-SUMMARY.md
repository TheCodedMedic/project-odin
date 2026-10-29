# Odin Writer Handbook - condensed (as of Oct 29, 2026 changelog)
Condensed by hand from the official handbook; the full text is not stored here because it is project documentation. Handbook = source of truth. Check its Changelog regularly.

## Pay and phases
- Hourly model since Oct 21, 2026. Base $40/hr (contract decides). Only Insightful-tracked time is paid; untracked time can't be added later. Hourly pay: Wednesdays for the prior Sat-Fri week (India time). Providers: Stripe (main), Wise.
- Onboarding: up to 3 paid hrs total (does not renew). First task: $150 on first submission + $250 when first approved (= the "$400"). Keep going without the timer if hours run out.
- Trial (tasks 2-4): 12 hrs allowance; each task reaching Review Approved adds 3 hrs. No tier bonus. After 3 Trial tasks approved -> Production. Rejected tasks don't count.
- Production tiers (reviewed daily after 3 newly resolved tasks): Throttled $40/hr, 40h/wk, 3 open tasks; Writer $55, 60h, 5; Super Writer $75, 80h, 10.
- Insightful (Workpuls): SSO with @mercor.expert, start "Glowstone-Odin - Task" timer, keep minimized, never show its window while recording. Don't track idle/waiting/breaks.
- Aim for ~1 task/day after onboarding. Max 4 reviews per task (initial + 3 resubmits), then rejected.
- App reimbursement: up to $50 per rolling 30 days, only after 1 approved task.

## Mac and desktop setup (technical requirements)
- Apple silicon or Intel; macOS 15+; 35 GB+ free; 16 GB RAM preferred; built-in display preferred (no native 4K/5K). Physical Mac only. No VPN / Private Relay (termination risk).
- TaskRecorder 2.4.4 (Intel build exists). Permissions: Accessibility, Screen Recording, Microphone. Xcode installed and Accessibility Inspector RUNNING (window closed with red button, never quit) during recording.
- Clock shows seconds. Dock on left/right, not hidden, indicators on. English system language.
- Empty Desktop, no widgets, built-in wallpaper, Do Not Disturb, fresh browser profile (Chrome/Safari/Firefox OK), Mac renamed (no real name). Optional separate "Recorder" macOS user.
- Change at least one UI element per recording (light/dark, wallpaper, accent colour, Dock size, resolution...). Cursor stays default.
- Test recording first; need >0.5 screenshots per second of video.

## Task rules
- Realistic professional workflow in your domain showing expertise + judgment ("friend with no expertise could do it?" -> too easy). Mostly mouse-driven. Variety between tasks (different objective/decision/method/flow, not just new names/data/app swap).
- 15:00-50:59 including intro and epilogue (reviewers tolerate to 54:59). At least 1 app, 2-3 ideal, each meaningful. Main app does most of the work.
- At least one final output must be created during the recording (a final output saved >30 min before recording fails).
- Idea (own words, no pasted AI text): Domain/Role, Goal (what + who uses it), Starting materials (+ source), Steps with app per step, Deliverable (+ how a reviewer can check it). Pick apps from list or "Other" with exact name. Approved idea locks; use "Revise idea" for material changes.
- Inputs: self-created, synthetic, Gemini-prepared before recording (note "AI-generated before recording" in Final Notes), or verified CC0/public domain. No watermarks (except Gemini), no (c) notices, no paywalled/unclear licence. Public GitHub OK for SWE/ML/DS.
- AI: only Gemini allowed, only BEFORE recording. No AI interaction, Google AI Overview/AI Mode, or AI features doing substantive work on camera.

## App status
- BANNED (new work): Godot, VSCodium, Inkscape, GIMP, Blender, MATLAB, Sublime Text, Photoshop, Ableton Live, ZBrush, Grammarly, Microsoft Whiteboard, Adobe Bridge, Adobe Animate, Unreal Editor, Telegram, KNIME, Reactotron, Craft, LiquidText, Media Encoder, Sublime Merge, Vital, Twinmotion, Figma, Adobe Lightroom, Autodesk FBX Review, Defold, KiCad, OpenVSP, anatomyapp, FL Studio, GameMaker, LTspice, Parallels Desktop, UCSF Chimera, VMD, Wolfram Mathematica, Substance 3D Stager, Sticky Notepad, Penpot, MohrPlotter, JASP, Windows (VM/remote, added Oct 29), TextExpander, TextEdit (only for creating metadata.rtf).
- LIMITED (<20% of the video): iTerm; RecipeKeeper, drawBook, Milanote (minor supporting use only). Background-only: Insightful, Splashtop Streamer.
- Allowed but prefer alternatives: Excel (recording issues - use Google Sheets), Preview, LibreOffice, Freeform, Stickies, Calendar, Terminal, Canva, Numbers, Reminders, Simplenote.
- Chrome, Safari, Firefox allowed. Word, PowerPoint, Premiere Pro, Illustrator allowed. Apps not on the list need no approval. Live list: https://odin-mercor1.vercel.app/validated-apps (per handbook).

## Before recording
- Goal text identical in 4 places: Studio approved Goal, TaskRecorder Task Description, opening Goal document (Word/Google Docs, NOT Notes/TextEdit), Metadata.rtf Request. No Approval ID. TaskRecorder Used Apps = approved app list.
- Metadata.rtf (made in TextEdit as RTF): Topology = every app visit in order, repeat on return, each labelled LOOKUP / CREATE / MODIFY; Request = Goal; Task Description = numbered high-level steps (apps, methods, deliverable).
- Launch/sign in/open files in all apps, position, then minimize. Never launch/set up apps after pressing Start. Quit everything else (Cmd+Tab check). Don't click the Downloads stack. Eject DMGs. No Studio/Slack/Guidelines/Mercor/Odin visible.
- PII: no real name/photo/email in app corners, browser profile, Finder paths (/Users/jane is fine), history, notifications. Use mercor.expert account or anonymised accounts. No iCloud/Apple ID creation.

## Recording
- Start with only the Goal doc behind TaskRecorder; Start Recording; minimize TaskRecorder immediately. Say: "I will be beginning my task soon. Here is the workflow I have in mind." (<20 s, don't read the Goal), minimize/close the Goal doc.
- One uninterrupted take, no pause. Narrate What + Where + Why (name controls and screen location; no "this/that/here"); announce every keyboard shortcut; English only; no profanity.
- Pause ~1 s after clicks; cursor as teaching pointer. Typing <=25% of video (35% coding/writing), no continuous typing >45 s. Silence: aim <=45 s, >60 s fails. Quiet room, steady volume.
- Windows: one clear active window or side by side; keep menu bar, clock, Dock visible; no full screen; don't cover one window by >25% for >30 s (popups of same app count).
- Small mistakes: say what, fix, verify, mention in epilogue. Restart only if the final result is affected or the flow is broken.
- Epilogue 3-4 min (max 4:00): outcome and verification, approach, problems and fixes, quality/limits, what you'd improve. Mouse may be still.

## Stop, package, submit
- Bring TaskRecorder forward, Stop; wait Stopping -> Archiving -> Idle. Show Recordings -> newest recording_TIMESTAMP.zip (don't edit/rename/unzip). Check video.mp4 start/middle/end, narration, screenshots count.
- Deliverables.zip: files named `input 1`, `artifact 1`, `final output 1` (lowercase, proper extensions; folders allowed for multi-file outputs). Metadata.rtf, video.mp4 and the original TaskRecorder zip are uploaded separately.
- Studio: upload the 4 files, list input sources (URL or "AI-generated before recording"), run both AutoQC checks (files+recording ~10 min; narration), fix or dispute (Dispute button + reason + timestamp) every Major flag, tick manual and PII checks, Final Confirmation, Submit for Review. Use "Run full AutoQC" not "Rerun failing".
- Major (blocking) examples: banned app >=10 s, limited app >=20%, window cover, Dock not visible at start/end, mouse still >90 s, typing over limit, silence >60 s, noise >40%, what/where/why <70% of counted actions, no Goal doc at start, intro >120 s, clock seconds missing, Accessibility Inspector not running, Used Apps mismatch, video not 15:00-54:59, no UI change, bad file names.
- Statuses: Idea Draft -> Checking Idea -> Idea Returned / Needs Review -> Idea Approved: Confirm Tech Setup -> (tech checklist) Start Recording -> submit -> Ready for review -> In Review -> Needs Edits (fix in same task, Submit for Review again) / Review Approved -> QC -> Ready for Delivery; Rejected = unusable, don't resubmit.

## Support
- #odin--helpdesk (tag @Maven): technical, tasking, onboarding. #odin--ideation: ideas. #odin--announcements: updates. Okta/Slack access: support@mercor.com. Don't DM reviewers. Private info seen in recording -> don't submit, re-record, tell helpdesk (no details).
- Pay/role issues: "Odin: Pay & Role Requests" form.

## Golden idea shape (from handbook examples)
"As a [role], [stakeholder need]. Using [App A] I will [method], then [App B] to [step], and [App C] to [deliver]. I will verify [check]. Deliver [named files]."
