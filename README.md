# RockGod® Build Engine Alpha V0.3

Static mobile-first customer prototype. It does not process payments, send emails, or store personal data.

## V0.3 changes
- Keeps Current Hair and Current Beard as separate focused steps.
- Normalises grayscale portrait treatment and improves beard framing/cropping on mobile.
- Adds stronger Target Hair / Target Beard section framing and plain-English prompts.
- Simplifies Nemesis wording to customer-observable symptoms: messy/fluffy, dry/rough, flat, hard to style, style does not last, rough beard, or maintenance.
- Keeps the new “What’s been holding you back?” barrier step.
- Adds a 16-slot Final Build portrait matrix in the code (`final-H-B.webp`). For V0.3 the slots intentionally use the same concept portrait so they can be replaced one-for-one with bespoke consistent images without changing the site logic.
- Keeps the detailed personalised Loadout summary.
- Expands the conversion screen with a £9.95 founding-offer test, illustrative crossed-out £24.95 reference price, trust cues, wallet-checkout mock buttons, and a “Continue Your Quest” email-capture demo.

## Important prototype caveats
- The crossed-out £24.95 is explicitly an illustrative prototype reference price, not an established previous selling price. Do not publish it as a real discount until it can be substantiated.
- Wallet buttons are visual demos only.
- Email is validated locally but not transmitted or stored.
- Product names, formulas, claims, sample sizes, postage and economics remain hypotheses pending Options/supplier validation.
- Supplier-dependent claims such as UK-made, vegan, cruelty-free, organic or similar are intentionally not asserted until confirmed.

## Publish
Upload `index.html` and the entire `assets/` directory to the root of the existing GitHub Pages repository and commit. GitHub Pages should redeploy automatically.
