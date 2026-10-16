# RockGod® Build Engine — Alpha V0.7

V0.7 is the commercial-refinement build created after a critical marketing / e-commerce review.

## Early Access signup

The Loadout result and final concept-offer screen include the Early Access CTA.
The final navigation button opens the same signup form. Character Creator answers
remain in browser memory and are not attached to signups.

- Existing onsite company: `VBguQ5` (tracking snippet preserved).
- Existing live Early Access popup: `RLQs3z`.
- Existing form list destination: `RwSVFa`.
- The CTA uses Klaviyo's supported `openForm` queue. Its hosted signup fallback
  uses the same list. Klaviyo continues to handle consent and confirmation emails.
- No private API key, new list, custom subscription endpoint or checkout is added.

Popup timing is managed in Klaviyo, not in this repository. In form `RLQs3z`,
open **Targeting & behavior** and use a 45-second time delay. To ensure visitors
get that browsing time, disable independent scroll/exit triggers that could open
the popup sooner. Preserve existing subscriber/dismissal suppression. Review
mobile visibility separately; the inspected live configuration targets desktop.
Publish the form after changing its settings. Do not delay the onsite tracking
script to control popup timing.

## What changed

- Opening proposition now explains the customer problem and payoff faster.
- Current Hair / Beard screens now ask for the closest **length**, reducing ambiguity.
- Happy Where I Am now gets its own Step 4 copy instead of being told it is working toward a future Build.
- Change route now labels the reveal clearly as **Target Build**.
- “Priority” language has been removed from the customer journey; the CTA now says **Face My Nemesis**.
- Maintain option is now **No Nemesis — just maintain my look**.
- Barrier answers are now optional; the customer can continue with none selected.
- Customer-facing “Bridge Loadout” language has been removed.
- Step 7 has been compressed:
  - Current → Target
  - Nemesis
  - reason for the recommendation
  - product cards
  - the real dynamic Equip Guide
- Target beard now produces explicit stage-aware guidance even when it should not yet add a beard product.
- Offer screen now shows a stylised **physical First Loadout** rather than repeating the target portrait.
- The £9.95 concept is framed as:
  - grooming minis
  - Equip card
  - next Quest
- Body wash add-on removed.
- Demo wallet buttons removed.
- Continue Your Quest is now a concrete **Quest Report**: what worked, what did not, what changed.
- Portrait loading is progressive rather than preloading all 24 image assets at launch.
- Friends/family testing prompts moved out of the customer page so they do not contaminate the blind test.

## Blind-test questions

Send the live link without explaining RockGod first. After the tester completes it, ask:

1. In the first 10 seconds, what did you think RockGod was offering?
2. Was Current Build → Target Build easy to understand?
3. What did “Nemesis” mean to you?
4. Were you able to answer the “holding you back” screen honestly, including skipping it?
5. Did the recommendation feel selected for you or generic?
6. Without looking back, what were your recommended products for and how would you use them?
7. What did you expect to physically receive for £9.95?
8. Would you spend your own £9.95 on that offer? Why / why not?
9. Did the physical First Loadout mock-up increase or reduce the perceived value?
10. Was any language too gamey, cheesy or forced?
11. Would you come back after trying the products to complete a Quest Report?

## Suggested GitHub commit

`RockGod Alpha V0.7 – commercial refinement and First Loadout offer`

Final formulas, mini volumes, product claims, packaging, postage and £9.95 unit economics remain separate supplier-validation work.
