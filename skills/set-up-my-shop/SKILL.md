---
name: set-up-my-shop
description: Set up a GiftcardLayers gift card shop step by step, from the first gift card to the link or website section that sells it. Use when the user wants to start selling gift cards with GiftcardLayers or finish an unfinished setup.
---

# Set up my shop

1. Call `get_account_overview`. Its `setup_steps` say what is done. Tell the user in one or two lines what is left.
2. Ask only for what you can't work out: the business, its website if it has one, what to sell and for how much. If the user shares a website, use it for the name, colours, tone and photos.
3. Do the open steps in this order, one at a time. After each one, show the result and the link, and ask before the next.
   - **Gift card**: `create_gift_card`. It starts off sale.
   - **Look**: follow the design-a-gift-card skill.
   - **Page**: `get_page_layout`, `patch_page_layout`, `set_buy_form_fields`; look at it with `render_page`.
   - **Getting paid**: only the user can connect Stripe. Give them the link from `start_action` (connect_stripe) and wait.
   - **Emails**: read with `get_email`, improve the texts, look with `render_page`.
   - **Selling**: follow the gift-cards-on-my-website skill, or give the hosted link from `get_share_codes`.
4. Ask for a clear yes before switching a gift card to on sale.

Prices, validity, tax, invoice and bank details come from the user. Don't invent them. When a tool answers with `needs_the_users_yes`, show the user `what_will_happen` and wait for their answer.
