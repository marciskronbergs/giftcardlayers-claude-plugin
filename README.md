# GiftcardLayers

Run your gift card shop from Claude. GiftcardLayers is a web app where spas, saunas, hotels, restaurants, salons and other service businesses sell their own gift cards. This plugin connects Claude to your account and adds four ready workflows.

## What you get

| Skill | What it does |
| --- | --- |
| Set up my shop | Goes through the setup with you, from the first gift card to the link you share |
| Design a gift card | Turns your brand into a gift card, looks at the real picture and fixes what is off |
| Gift cards on my website | Adds a gift card section, a page or a buy button to your site, also in a code project |
| Monthly check | A short look at sales, undelivered emails, open balances and what to improve |

## Install

In Claude Code: `/plugin install giftcardlayers --marketplace marciskronbergs/giftcardlayers-claude-plugin`

## What you need

A GiftcardLayers account (the Free plan works): https://giftcardlayers.com/signup. The first time a skill needs your shop, Claude opens the GiftcardLayers sign-in page and you press Allow.

## What it connects to

- One remote server, `https://giftcardlayers.com/mcp`, run by GiftcardLayers, with OAuth sign-in. The plugin contains no keys or secrets.
- The plugin runs no scripts, hooks or local programs. Its skills are text instructions.
- Claude can read and change the gift cards, pages, emails, settings and orders of the account you sign in with. It can also read your buyers' order details when you ask about them.
- Redeeming, deleting, emailing customers and other risky steps wait for your yes. Claude can't pay, refund or move money.
- "Gift cards on my website" edits files in your own project only when you ask it to.

Make the connection view-only or remove it at any time in GiftcardLayers: Settings, Connect Claude. Privacy: https://giftcardlayers.com/privacy

## Try it

- "Set up my gift card shop. My website is example.com."
- "Design a €100 massage gift card in my brand colours and show me the picture."
- "Add my gift cards to the /gift-cards page of this Next.js project."
- "Do the monthly check of my gift card shop."

Help: https://giftcardlayers.com/claude-gift-card-mcp or support@giftcardlayers.com
