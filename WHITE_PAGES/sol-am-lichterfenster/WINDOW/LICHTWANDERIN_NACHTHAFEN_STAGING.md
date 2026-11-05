# Lichtwanderin im magischen Nachthafen — staged, NOT live
5 November 2026

This branch is intentionally a non-live staging area. The existing official live pane is unchanged.

- Unchanged verified official live backup: `BACKUP_window_2026-11-05_before_lichtwanderin.html` — Git blob `7a9f97ddc7b980222bb9de76c65fe8c482248113`.
- Additive complete HTML draft: `window_lichtwanderin_nachthafen_preview.html`.
- Missing required binary asset: `lichtwanderin_nachthafen_2026-11-05.gif` (the original 508×508 animated GIF, 6 frames, 2.1-second loop). SHA-256: `92a379a7b2096ec1a9913347fd01eb2930122abf1d3d659469dcda2d90fc8a9b`.
- The existing green-sail element (`#lw-scene`) and interactive controls remain in place in the draft.
- The new night scene is a second figure placed under the existing green-sail scene. It makes no World API calls.
- A local preview ZIP containing the exact GIF, poster and independent HTML test page was delivered separately in ChatGPT.
- Do NOT ship or merge the HTML without adding the GIF as a sibling asset, testing the live pane's interactions and responsiveness, and verifying its authorized Postmark deployment path.
- Reduced-motion: the staged full HTML falls back to the original green-sail media image; local preview ZIP uses a still frame from the GIF.
- Rollback: restore the backed-up `window.html` content / original git blob, not the fork's older Halloween-era version.

Status: FILE BACKED UP; ADDITIVE HTML DRAFT CREATED; ORIGINAL GIF NOT YET UPLOADED; **LIVE PANE NOT MODIFIED**.
