# Kadife creative library

Real, client-provided ad creative for the Meta funnel, organized by SKU and funnel stage so future
drops from the design team have an obvious place to land. Drop new files straight into the matching
`<sku>/<stage>/` folder and add a row below — nothing here is generated except where marked.

Meta ad account: `998707789870147` ("Kadife SD"). Live campaigns this maps to: `Actives Education
(Awareness) — TOFU`, `D-Tan + Glow Nectar (Traffic) — MOFU`, `Hydro Barrier + Oil Balance (Traffic)
— MOFU`. **Update 2026-09-21: TOFU is now ACTIVE** (campaign, ad set, and all 4 TOFU ads) — see the
new item at the bottom of Next steps. MOFU/BOFU remain PAUSED.

## Index

| SKU | Stage | File | Source | Status |
|---|---|---|---|---|
| D-Tan Pearl BW | TOFU | `d-tan-pearl-bw/tofu/why-sulfate-free.jpg` | Design team, WhatsApp 2026-09-19 | Ready |
| D-Tan Pearl BW | MOFU | `d-tan-pearl-bw/mofu/hero-still-scrubbing-tan-off-gemini.jpg` | Generated this session (Gemini, `gemini-3-pro-image`, real product photo as reference) | Ready — no real asset has surfaced for this slot yet |
| Glow Nectar FW | TOFU | `glow-nectar-fw/tofu/why-sulfate-free.jpg` | Design team, WhatsApp 2026-09-19 | Ready |
| Glow Nectar FW | MOFU | `glow-nectar-fw/mofu/everything-skin-waiting-for.png` | Design team, shared in chat 2026-09-19 | Ready |
| Glow Nectar FW | MOFU | `glow-nectar-fw/mofu/brightening-face-wash-niacinamide.png` | Design team, shared in chat 2026-09-19 | Ready — 2nd MOFU variant, good for an A/B test |
| Hydro Barrier FW | TOFU | `hydro-barrier-fw/tofu/why-sulfate-free.jpg` | Design team, WhatsApp 2026-09-19 | Ready |
| Hydro Barrier FW | MOFU | `hydro-barrier-fw/mofu/ugc-face-wash-demo.mov` (10s, 1080x1920) | Real UGC, Downloads `kadife bodywash ugc 6.mov` (filename is generic — verified by frame content: real Hydro Barrier FW bottle visible on counter) | Ready — video ad object not yet built |
| Oil Balance FW | TOFU | `oil-balance-fw/tofu/why-sulfate-free.jpg` | Design team, WhatsApp 2026-09-19 | Ready |
| Oil Balance FW | TOFU | `oil-balance-fw/tofu/animated-explainer-oil-vs-pores.mp4` (47.6s, 720x1280) | Real 3D-animated explainer, Downloads `kadife oil face wash.mp4` | Ready — video ad object not yet built |
| Oil Balance FW | MOFU | `oil-balance-fw/mofu/oily-skin-wash-it-off.png` | Design team, shared in chat 2026-09-19 | Ready |
| Oil Balance FW | MOFU | `oil-balance-fw/mofu/benefit-25pct-off.png` | Design team, shared in chat 2026-09-19 | **Confirmed live 2026-09-19 (user): 25% off applies to all face washes and body washes** — usable in ads. Same claim is fair to use in Glow Nectar FW / Hydro Barrier FW / D-Tan Pearl BW copy too, not just this image |
| Glow Radiance Pearl BW | TOFU | `glow-radiance-pearl-bw/tofu/why-sulfate-free.jpg` | Design team, WhatsApp 2026-09-19 | No Meta campaign exists for this SKU yet — filed for whenever it's added |
| Intense Hydrating Moisturiser | — | `other-products/intense-hydrating-moisturiser/ugc-application-demo.mp4` (20.6s, 1080x1920) | Real UGC, Downloads `KADIFE UGC 10.mp4` | Not one of the 4 funnel SKUs — filed correctly rather than discarded |

## Known gaps
- Nothing else open — every TOFU and MOFU slot for the 4 live-campaign SKUs (D-Tan Pearl, Glow
  Nectar FW, Hydro Barrier FW, Oil Balance FW) now has a real or generated asset.
- BOFU (`Retarget & Convert`) is intentionally held back per the funnel strategy doc — no warm
  audience yet. The 25%-off Oil Balance image (offer confirmed live) is a plausible BOFU candidate
  once that activates.
- **Broken destination link — found and fixed (2026-09-19)**: the original 8 in-scope ads (built
  before this library existed) had NO working destination at all — confirmed by the user actually
  clicking the CTA and nothing happening, not just an API-field gap. Root cause: they were built as
  `SHARE`-type/page-post creatives with no `link_data.link`. Fixed by building 8 new creatives with
  `link_url` set directly, then 8 new **ads** referencing them (creatives are immutable — a new ad
  was required, editing in place isn't possible) — confirmed working via the ad's own Destination →
  Website URL field in Ads Manager (the ad-preview iframe turned out to be non-interactive/useless as
  a test either way, which is what made this take two attempts to pin down). New ad IDs: D-Tan Pearl
  MOFU `120253117505650316`, D-Tan TOFU `120253117508520316`, Glow Nectar MOFU `120253117509850316`,
  Glow Nectar TOFU `120253117510180316`, Hydro Barrier MOFU `120253117510810316`, Hydro Barrier TOFU
  `120253117511280316`, Oil Balance MOFU `120253117512140316`, Oil Balance TOFU `120253117512620316`
  — all PAUSED. The 8 original broken ads are archived. These fixed ads still use the OLD flat
  product photos (image_hash reused as-is) — the richer images below are NOT swapped in yet; that
  needs real public image hosting (a private `claude.ai/artifact/...` URL was tried and confirmed
  NOT fetchable by Meta's servers — "image could not be downloaded").
- Two SKUs from the earlier build (`D-Tan Polish Mask`, `Glow Nectar Moisturizer` — both different
  products from this library's SKUs) are still live in the MOFU1 ad set with the same broken-link
  bug, untouched; still waiting on the user's keep-or-swap call.

## Not included here (checked, not relevant)
- `KADIFE A+.zip` (Downloads) — the OLD Kadife product line's A+ photography (De-Tan mask jar,
  a different generic face wash tube). Verified by opening the actual images, not by folder name.
- `kadife mask ugc 3.mov`, `Double shot radiance serum...mp4` — different product lines.
- `real estate next ugc 1.mp4` — a different client's file.

## Next steps (not done in this pass)
1. ~~Confirm the Oil Balance 25%-off offer status~~ — done, confirmed live account-wide on face washes
   and body washes.
2. ~~Fix the broken Amazon destination link~~ — done, see Known Gaps above. 8 new, working ads live
   (PAUSED) under their real ad sets; 8 old broken ones archived.
3. Solve real public image hosting, then swap this library's richer images into the 8 fixed ads
   (currently still on the old flat product photos) — needs a genuinely public direct-fetch URL, not
   a private Artifact link. **Re-confirmed 2026-09-21**: tried again (Artifact asset store with
   `capabilities: {assets: {}}` declared) — still organization-internal, not fetchable by Meta
   ("unsupported"/not attempted after the earlier session's own "image could not be downloaded"
   result). Still unsolved; needs a real image host (S3/Cloudinary/etc.).
4. Video assets (Hydro Barrier UGC, Oil Balance animated explainer) need a video ad creative object,
   not the static-image one — flagged, not built.
5. Decide whether `D-Tan Polish Mask` and `Glow Nectar Moisturizer` (different SKUs, already live in
   MOFU1 from the earlier build, same broken-link bug, not yet fixed) stay in the funnel or get
   swapped for this library's SKUs.
6. **2026-09-21 — TOFU activated.** Campaign `120252851661440316` (Actives Education, ₹120/day CBO),
   ad set `120253112502670316`, and all 4 TOFU ads (Oil Balance `120253117512620316`, Hydro Barrier
   `120253117511280316`, Glow Nectar `120253117510180316`, D-Tan `120253117508520316`) are now
   `status: ACTIVE` (effective_status was PENDING_REVIEW/IN_PROCESS right after activation — normal,
   Meta's ad review). MOFU and BOFU deliberately left PAUSED (no warm audience yet). Oil Balance ASIN
   confirmed by the user: `B0HH7CG4W4` (https://www.amazon.in/dp/B0HH7CG4W4 — not yet a real Amazon
   Attribution tag, just the bare PDP link). Instagram (`instagram.com/kadife_kare`) still not linked
   to this ad account — user connecting it manually via Business Settings. A separate, unused
   duplicate TOFU/MOFU/BOFU campaign set was created earlier in the same session before this history
   was found (`120253137206390316`/`...890316`/`...350316`, "Facewash & Body Wash — Amazon...") — no
   creative attached, safe to delete.
