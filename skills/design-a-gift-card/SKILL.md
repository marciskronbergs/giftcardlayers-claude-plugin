---
name: design-a-gift-card
description: Design or redesign a gift card in GiftcardLayers so it fits the business's brand, checking the real rendered picture. Use when the user wants a new gift card look, or their logo, colours or photos on a gift card.
---

# Design a gift card

1. Find the card with `list_gift_cards`, or create one with `create_gift_card` (it starts off sale). Read `get_card_design` and `get_branding`.
2. Read `get_design_guide` with topics `design_principles` and `card_designer`, and `get_design_options` with area `card`.
3. Agree on one line first, for example: "Quiet Nordic spa: warm stone and deep green, serif name, lots of space."
4. Set the colours and font with `set_branding`, then the picture with `set_card_design`. Prefer colour tokens over fixed colours, two fonts at most, one idea per card.
5. Photos and logos must be the business's own: `import_image` from its website, or the upload page from `list_uploads`.
6. Call `render_gift_card` and look: contrast, cut-off or overlapping text, crooked spacing, empty corners. Fix and look again, up to three rounds.
7. Show the user the picture and the preview link. Ask before putting it on sale.

If an answer lists `refused` values, those were not saved: choose an allowed value and say so.
