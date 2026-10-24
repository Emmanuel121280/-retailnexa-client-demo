# RetailNexa mobile and interaction repair

Replace the repository root `index.html` with this revised file and redeploy GitHub Pages. This fixes the missing mobile menu, iPhone navigation, touch-target sizing, narrow-screen grids, chat control layout, and industry selection accessibility.

## What works on a static website
- All anchor navigation and mobile menu
- Industry selector tabs
- Searchable feature catalogue
- Simulated WhatsApp chat replies
- Email link (requires visitor to have an email app configured)

## What requires backend services
- Customer signup/login
- Real POS, payments, AI, orders, WhatsApp API, subscriptions and live inventory

## Smoke-test after publish
1. Check 375px and 390px viewport widths; no horizontal scrolling.
2. Tap menu -> Features -> menu collapses and page scrolls correctly.
3. Change Restaurant/Hotel/Logistics tabs and verify module lists change.
4. Type `rice` in feature search and see filtered features.
5. Enter `Do you have rice?` and tap Send demo message.
6. Tap Request a demo and Email RetailNexa (requires mail application).
7. Verify all navigation anchors resolve to section ids.
8. Confirm GitHub Pages reports latest deploy and public URL serves updated index.html.

No live backend or GitHub deployment is included in this package.
