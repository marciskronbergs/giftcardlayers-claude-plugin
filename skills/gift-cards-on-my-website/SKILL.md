---
name: gift-cards-on-my-website
description: Put GiftcardLayers gift cards on the user's own website as a section, a full page or a buy button, in a website builder or directly in a code project (HTML, React, Next.js, Vue, Astro and others). Use when the user wants to sell or embed their GiftcardLayers gift cards on their site.
---

# Gift cards on my website

1. Ask what to show (one gift card or several) and where, if it isn't clear. Use `list_gift_cards` and `list_collections`; make a section with `create_collection` if several cards are needed and none exists.
2. Call `get_share_codes` for it. Pick one:
   - **Section**: the live gift cards inside a page. Best for most sites.
   - **Page**: the whole gift card page as its own page, such as /gift-cards.
   - **Button**: a link that opens the purchase.
   - **Iframe only**: for builders that block scripts.
3. Use the returned code as it is. The cards stay live, so later changes in GiftcardLayers show without new code.

## Website builder

Give the code and the steps for their builder: WordPress Custom HTML block, Wix Embed HTML, Squarespace Code block, Shopify Custom Liquid, Webflow Embed.

## Code project

1. Find how the project makes pages, and follow its routing, components and styles.
2. Put the returned element in the page. Load `https://giftcardlayers.com/widget/buy.js` once, the way the framework loads third-party scripts (Next.js: `next/script`; elsewhere a script tag with `async`).
3. In a client-side router the script may already be loaded when the page appears: call `window.GiftcardLayersBuy?.scan()` after the page mounts.
4. If the site has a Content Security Policy, allow `https://giftcardlayers.com` in `script-src` and `frame-src`.
5. Add a menu link if the user wants one. Run the project's build, open the page and check the cards show on desktop and phone width.

No key or secret is needed in the code. Don't commit or deploy unless the user asks.
