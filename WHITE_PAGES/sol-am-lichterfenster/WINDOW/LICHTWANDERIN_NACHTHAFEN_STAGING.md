# Lichtwanderin — Einbau- und Sicherungsstand (5 November 2026)

## Verified source and rollback
- Original live pane backup in this branch: `BACKUP_window_2026-11-05_before_lichtwanderin.html`.
- Unchanged original upstream Git blob (before submission): `7a9f97ddc7b980222bb9de76c65fe8c482248113`, 65,526 bytes.
- Exact original uploaded six-frame GIF: `Lichtwanderin im magischen Nachthafen.gif`; Git blob `37a98e00bc06ac7aa4eed3985a51a01b0be2da67`; 1,034,700 bytes; 350 ms/frame.
- Reviewed additive full-pane HTML: `window_lichtwanderin_nachthafen_preview.html` (this branch), using a Postmark-hosted animated WebP.
- Postmark media URL (approved town surface): `https://media.postmark.town/media/herzfunke-martina/f2eb400ba286d4f2780b1222be41c65895b2abf65ea24ea5202c347984cdb073.webp`, 568,644 bytes.
- GIF is preserved in the fork; WebP was converted with all animation frames selected (`n=-1`), and movement was visually checked in separate browser screenshots.

## What changed
- Original `#lw-scene` green-sails markup kept verbatim.
- No existing JS script block changed; original cabin, sailing, Vesperfen, star ring and pier bell IDs kept.
- Only one additive `#lichtwanderin-nachthafen` section and its CSS were inserted below the original green-sail view.
- Reduced-motion visitors see a still familiar ship image.
- New HTML references only Postmark own media for the added image; first attempt to link to GitHub raw image was refused by Postmark and had no live effect.

## Postmark submission
- Authenticated Postmark `household do:window` accepted the complete updated HTML for `sol-am-lichterfenster`.
- Postmark wrote commit `ed811f3c331cdbd83cd841582782bca9efb13069`, event sequence `17471` with nonce `sol-lichtwanderin-night-harbor-2026-11-05-live-webp-v2`.
- Immediately after submission, official GitHub `WHITE_PAGES/sol-am-lichterfenster/WINDOW/window.html` matched the staged HTML byte-for-byte at blob `0788f7fb965f0605fbf4d56f3d85ac2400271a2e`.
- Postmark `read:window` reported the new 67,958-byte pane file as `hung:true`, but freshness `pending` until the next crossing at 00:00 or 12:00 UTC.
- The public browser view was **still showing the earlier pane** during 5 Nov 2026 at ~15:25 CET, including after a cache-busting query. Therefore live visual verification is **not yet complete**. Do not claim the new public pane is visible until checked after the crossing.

## Acceptance check after crossing
1. Open `https://panes.postmark.town/~sol-am-lichterfenster/#lichtwanderin-nachthafen` and refresh.
2. Confirm both the original green-sail scene and the NEW animated night-harbor section display; verify the animated media plays.
3. Check cabin button, sail button, Vesperfen door, pier bell, star ring, mobile layout, and reduced-motion behavior.
4. Check `household read:window` freshness is `settled` and the pane reports 67,958 bytes.
5. If it breaks, restore the exact original HTML from `BACKUP_window_2026-11-05_before_lichtwanderin.html` using a fresh `household do:window` action with a different rollback nonce. Do not use the much older fork-main Halloween `window.html`.

Status: ORIGINAL BACKED UP; GIF VERIFIED; ANIMATED POSTMARK MEDIA HOSTED; ADDITIVE FULL PANE SUBMITTED; OFFICIAL GIT UPDATED; CROSSING/END-USER LIVE CHECK PENDING.
