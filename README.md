# Kadife creative library

Real, client-provided ad creative for the Meta funnel, organized by SKU and funnel stage so future
drops from the design team have an obvious place to land. Drop new files straight into the matching
`<sku>/<stage>/` folder and add a row below — nothing here is generated except where marked.

Meta ad account: `998707789870147` ("Kadife SD"). Live campaigns this maps to: `Actives Education
(Awareness) — TOFU`, `D-Tan + Glow Nectar (Traffic) — MOFU`, `Hydro Barrier + Oil Balance (Traffic)
— MOFU`. TOFU is ACTIVE. MOFU/BOFU remain PAUSED (no warm retargeting audience yet).

**Public asset host**: this whole folder is also pushed to a public GitHub repo —
`https://github.com/genzmarketing82-ctrl/kadife-ad-assets` (raw file URLs at
`https://raw.githubusercontent.com/genzmarketing82-ctrl/kadife-ad-assets/main/<path>`) — so images/videos
here can be uploaded to Meta via a public URL. This is how the "no public image host" blocker below got
solved on 2026-09-21. Push any new file added here so it's fetchable the same way.

## Index

| SKU | Stage | File | Source | Status |
|---|---|---|---|---|
| D-Tan Pearl BW | TOFU | `d-tan-pearl-bw/tofu/why-sulfate-free.jpg` | Design team, WhatsApp 2026-09-19 | Ready — used in fixed-link ad |
| D-Tan Pearl BW | TOFU | `d-tan-pearl-bw/tofu/flat-bottle-alt.jpg` | Client, 2026-09-21 | Filed as backup — not built into an ad this pass |
| D-Tan Pearl BW | MOFU | `d-tan-pearl-bw/mofu/hero-still-scrubbing-tan-off-gemini.jpg` | Generated (Gemini, `gemini-3-pro-image`, real product photo as reference) | **Built into ad `120253140411850316` (PAUSED) 2026-09-21** |
| D-Tan Pearl BW | MOFU | `d-tan-pearl-bw/mofu/pearl-glow-story-1080x1920.png` (+ `-9x16.png`, native 3072x5504 — too large for Meta, 1080x1920 used) | Client, 2026-09-21 | **Built into ad `120253140571710316` (PAUSED) 2026-09-21 — Stories/Reels variant** |
| Glow Nectar FW | TOFU | `glow-nectar-fw/tofu/why-sulfate-free.jpg` | Design team, WhatsApp 2026-09-19 | Ready — used in fixed-link ad |
| Glow Nectar FW | MOFU | `glow-nectar-fw/mofu/everything-skin-waiting-for.png` | Design team, shared in chat 2026-09-19 | **Built into ad `120253140412600316` (PAUSED) 2026-09-21** |
| Glow Nectar FW | MOFU | `glow-nectar-fw/mofu/brightening-face-wash-niacinamide.png` | Design team, shared in chat 2026-09-19 | **Built into ad `120253140413520316` (PAUSED) 2026-09-21 — A/B variant** |
| Glow Nectar FW | MOFU | `glow-nectar-fw/mofu/gentle-glow-story-1080x1920.png` (+ `-9x16-4k.png`, too large for Meta, 1080x1920 used) | Client, 2026-09-21 | **Built into ad `120253140568230316` (PAUSED) 2026-09-21 — Stories/Reels variant** |
| Hydro Barrier FW | TOFU | `hydro-barrier-fw/tofu/why-sulfate-free.jpg` | Design team, WhatsApp 2026-09-19 | Ready — used in fixed-link ad |
| Hydro Barrier FW | MOFU | `hydro-barrier-fw/mofu/ugc-face-wash-demo.mov` (10s, 1080x1920) | Real UGC, Downloads `kadife bodywash ugc 6.mov` (filename is generic — verified by frame content: real Hydro Barrier FW bottle visible on counter) | **Built into video ad `120253140417130316` (PAUSED) 2026-09-21** |
| Oil Balance FW | TOFU | `oil-balance-fw/tofu/why-sulfate-free.jpg` | Design team, WhatsApp 2026-09-19 | Ready — used in fixed-link ad, also swapped into richer-image ad `120253140409500316` |
| Oil Balance FW | TOFU | `oil-balance-fw/tofu/flat-bottle-alt.jpg` | Client, 2026-09-21 | Filed as backup — not built into an ad this pass |
| Oil Balance FW | TOFU | `oil-balance-fw/tofu/animated-explainer-oil-vs-pores.mp4` (47.6s, 720x1280) | Real 3D-animated explainer, Downloads `kadife oil face wash.mp4` | **Built into video ad `120253140411240316` (PAUSED) 2026-09-21** |
| Oil Balance FW | MOFU | `oil-balance-fw/mofu/oily-skin-wash-it-off.png` | Design team, shared in chat 2026-09-19 | **Built into ad `120253140414710316` (PAUSED) 2026-09-21** |
| Oil Balance FW | MOFU | `oil-balance-fw/mofu/benefit-25pct-off.png` | Design team, shared in chat 2026-09-19 | **Built into ad `120253140415390316` (PAUSED) 2026-09-21 — 25%-off A/B variant.** 25% off confirmed live account-wide on face washes and body washes |
| Oil Balance FW | MOFU | `oil-balance-fw/mofu/acne-care-story-1080x1920.png` (+ `-9x16.png`, too large for Meta, 1080x1920 used) | Client, 2026-09-21 | **Built into ad `120253140569610316` (PAUSED) 2026-09-21 — Stories/Reels variant** |
| Glow Radiance Pearl BW | TOFU | `glow-radiance-pearl-bw/tofu/why-sulfate-free.jpg` | Design team, WhatsApp 2026-09-19 | No Meta campaign exists for this SKU yet — filed for whenever it's added. ASIN confirmed 2026-09-21: `B0H8DY95DF` |
| Intense Hydrating Moisturiser | — | `other-products/intense-hydrating-moisturiser/ugc-application-demo.mp4` (20.6s, 1080x1920) | Real UGC, Downloads `KADIFE UGC 10.mp4` | Not one of the 4 funnel SKUs — filed correctly rather than discarded |

## Confirmed Amazon ASINs (2026-09-21)
- Oil Balance Face Wash — `B0HH7CG4W4` — https://www.amazon.in/dp/B0HH7CG4W4
- Hydro Barrier Face Wash — `B0HH7GCPV2` — https://www.amazon.in/dp/B0HH7GCPV2
- Glow Nectar Face Wash — `B0HH7BH8LX` — https://www.amazon.in/dp/B0HH7BH8LX
- D-Tan Pearl Body Wash — `B0HH7G4FS2` — https://www.amazon.in/dp/B0HH7G4FS2 (corrected 2026-09-24;
  was wrongly recorded as `B0H8S7XHFL` — that ASIN is stale/unlinked, confirmed via live SP-API +
  the user's own storefront search. **The live Meta ad below still links to the old ASIN.**)
- Glow Radiance Pearl Body Wash (no campaign yet) — `B0H8DY95DF` — https://www.amazon.in/dp/B0H8DY95DF

Kadife only sells 3 face washes (Oil Balance, Hydro Barrier, Glow Nectar) and 2 body washes (D-Tan
Pearl, Glow Radiance Pearl) as real standalone products. "D-Tan Polish Mask" and "Glow Nectar
Moisturizer" are NOT real products — see Known gaps.

## Known gaps
- **Image hosting — solved 2026-09-21.** Public GitHub repo (`kadife-ad-assets`, see top of this file)
  gives Meta-fetchable raw URLs. Note: Meta rejects the native ~3072x5504 4K story-card renders as
  "Resized Image Too Large" — use the 1080x1920 versions instead.
- **Broken destination link — fixed 2026-09-19.** Original 8 ads had no working destination
  (`SHARE`-type creatives with no `link_data.link`). Fixed with 8 new creatives carrying `link_url`
  directly + 8 new ads (creatives are immutable). Those 8 fixed ads are still live at their original
  IDs, now further **superseded by richer-image versions built 2026-09-21** (see Index above) — both
  sets currently coexist, PAUSED, pending the user picking a final set per ad set.
- `D-Tan Polish Mask` and `Glow Nectar Moisturizer` — confirmed 2026-09-21 by the user these are not
  real standalone products. Their old broken-link ads (`120253117712020316`, `120253117710870316`)
  are **archived**, not fixed.
- A duplicate, unused TOFU/MOFU/BOFU campaign set (`120253137206390316`/`...890316`/`...350316`,
  "Facewash & Body Wash — Amazon...") had no creative attached — **archived 2026-09-21**.
- BOFU (`Retarget & Convert`) still intentionally held back — no warm audience yet.

## Not included here (checked, not relevant)
- `KADIFE A+.zip` (Downloads) — the OLD Kadife product line's A+ photography (De-Tan mask jar,
  a different generic face wash tube). Verified by opening the actual images, not by folder name.
- `kadife mask ugc 3.mov`, `Double shot radiance serum...mp4` — different product lines.
- `real estate next ugc 1.mp4` — a different client's file.

## Next steps
0. **Meta catalog (`Kadife SD`, ID `1794548301889007`) is being populated (2026-09-24)** with a real
   product feed (5 SKUs, live Amazon MAIN images + current prices) — was created but had zero
   products before this. See account-info.md for the full note.
0b. **Fix needed, not yet done**: the live Meta ad for D-Tan Pearl Body Wash still links to the
   stale ASIN `B0H8S7XHFL` instead of the real current one, `B0HH7G4FS2` (found 2026-09-24). This
   is a running-ad destination-link change — needs the user's go-ahead before editing.
1. **User review needed**: 14 new PAUSED ads sit alongside the 8 already-live "fixed-link" ads across
   TOFU/MOFU (image swaps, 2 video ads, 3 Stories/Reels variants). Decide which to activate vs. archive
   the older flat-photo duplicates once reviewed in Ads Manager.
2. Instagram (`instagram.com/kadife_kare`) still not linked to ad account `998707789870147` — user
   connecting manually via Business Settings; re-check with `ads_get_ig_accounts` before building any
   IG-specific placement.
3. BOFU activation once a warm retargeting audience exists — the 25%-off Oil Balance image is a
   plausible BOFU candidate.
4. Amazon Attribution tags not yet set up — all links above are bare PDP links, no conversion signal
   captured on the Meta side yet (no pixel either).
