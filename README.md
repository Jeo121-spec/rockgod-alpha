# RockGod® Build Engine Alpha V0.4.1.7

Static mobile-first customer prototype. It does not process payments, send emails, or store personal data.

## V0.4.1.7 focus
This release is the visual-integration pass requested after the V0.3 phone review. It deliberately does **not** redesign the product-recommendation decision framework yet.

### What changed
- Unified the grayscale portrait treatment for Current Hair, Current Beard, Target Hair and Target Beard.
- Fixed mobile beard framing so the full beard remains visible rather than being cropped by the card.
- Added 16 working Final Build images (`final-H-B.webp`): 4 hair states × 4 beard states.
- Step 4 now dynamically displays the selected hair + beard combination.
- The same selected Final Build now carries through to Step 7 / the Loadout summary.
- The same selected Final Build also appears on the £9.95 founding-offer screen, preserving the customer's visual Build through conversion.
- Kept the stronger Target Hair / Target Beard framing, simplified Nemesis wording, barrier step, £9.95 offer, wallet mock buttons and Continue Your Quest route.

## Deliberately next
- Recommendation decision framework: map Current Build + Target Build + Nemesis + Barrier to a justified product/routine recommendation.
- Final supplier-confirmed product names, formulas, claims, costs and sample sizes.
- Real checkout / Apple Pay / Google Pay integration via the eventual commerce platform.
- Final production-grade portrait art can replace the 16 Alpha composites one-for-one without changing the website logic.

## Important prototype caveats
- £24.95 is an illustrative prototype reference price, not an established previous selling price. Do not publish it as a real discount until it can be substantiated.
- Wallet buttons are visual demos only.
- Email is validated locally but not transmitted or stored.
- Product recommendations remain provisional until the decision framework is designed and supplier/product testing is complete.
- Supplier-dependent claims such as UK-made, vegan, cruelty-free or organic are intentionally not asserted until confirmed.

## Publish
Upload `index.html` and the entire `assets/` directory to the root of the existing GitHub Pages repository and commit with a message such as `Update to RockGod Alpha V0.4.1.7`. GitHub Pages should redeploy automatically.


## V0.4.1.7 micro-patch
- Beard reference portraits now use a muted grayscale / lower-contrast treatment to better match the Hair portrait set across Current Beard, Target Beard and downstream reference cards.
- No flow, recommendation, copy or commercial logic changes in this patch.


## V0.4.1.7 locked visual treatment

Approved portrait rule:
- same face identity and lighting across hair and beard rows
- eyes and nose softened/recessive
- hair/beard remain the strongest visual feature
- black/charcoal background with muted grayscale portrait treatment
- this approved treatment is now embedded in the hair and beard assets


## Definitive V0.4.1.7 asset fix

This package is the corrected V0.4.1.7 release.

- Approved softened hair and beard assets are embedded in `/assets`.
- No additional beard-only CSS darkening/filter is applied.
- Hair and beard rows now use the same visual treatment in the website.
- Use this package instead of the earlier V0.4.1.7 / V0.4.1.7 LOCKED ZIPs.

## V0.4.1.7 cache-busting patch

The approved softened portrait assets were already present in V0.4.1.3, but GitHub Pages / mobile browsers could continue serving older images because the filenames were unchanged.

V0.4.1.7 fixes this by using new versioned image filenames for:
- hair assets
- beard assets
- all 16 Final Build portraits

This forces the browser to retrieve the corrected images rather than reuse cached copies.

## V0.4.1.7 image-path fix

All image files used by the prototype now sit in the repository root alongside `index.html`.
This removes the possibility of a missing `/assets/` folder during browser-based GitHub uploads.

When uploading this version, select **every file inside this folder** and upload them together.

## V0.4.1.7 — real 16-image Final Build matrix

This version replaces the ghosted/composited Final Build portraits with 16
single finished portraits:

- 4 hair states: Bald/Shaved, Short, Medium, Long
- 4 beard states: Clean Shaven, Stubble, Short, Long
- each Hair × Beard result is a standalone portrait, not an overlay
- the selected portrait is reused on the Final Build, Built for Your Quest,
  and First Loadout screens

Also:
- the Welcome screen buttons “Looking to Change” and “Happy Where I Am”
  now explicitly use the same Arial/Helvetica UI font as the rest of the page.

## V0.4.1.7 — Final Build display-quality patch

The 16 Final Build portraits are currently lower-detail source assets than the
hair/beard reference portraits. This patch stops the centre image being enlarged
beyond the point where it looks soft/pixelated.

- desktop centre portrait capped at 220px wide
- mobile centre portrait capped at 220px wide
- summary grid rebalanced so the centre portrait still reads as the hero image
- no changes to journey logic or portrait selection
