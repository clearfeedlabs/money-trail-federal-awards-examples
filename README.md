# USAspending Scraper: Federal Contract & Grant Award Alerts: examples

Follow the federal money: new and changed contracts, grants, loans and IDVs from the official USAspending.gov API, filtered by keyword, agency, recipient, NAICS, state or amount. Change alerts + recipient parent-company add-on.

This repo shows how to call the [Money Trail: Federal Contract & Grant Alerts](https://apify.com/clearfeedlabs/money-trail-federal-awards) Apify Actor from JavaScript or Python, and what the output looks like.

## What's new
- Free competition & recompete fields on contract rows: offers received, extent competed, set-aside, pricing type, potential end date, recompete window.

## Use cases
- Government contractors finding recompete and teaming opportunities
- BD teams tracking competitors' new awards
- Grant-funded organisations watching agency funding
- Journalists and analysts following federal spending

## Quick start
1. Create a free Apify account and copy your API token from Settings > Integrations.
2. Set it as an environment variable: `export APIFY_TOKEN=...` (never commit it).
3. Edit `input.json`, then run one of:
   - JavaScript: `npm i apify-client && node run.mjs`
   - Python: `pip install apify-client && python run.py`

## Output fields (first of many)
`rowType`, `awardId`, `awardKey`, `awardCategory`, `awardType`, `recipientName`, `recipientId`, `amount`, `totalOutlays`, `awardingAgency`, `awardingSubAgency`, `fundingAgency`, `startDate`, `endDate`, `lastModified`, `description`, `naics`, `naicsDescription`

See `sample-output.json` for one trimmed record.

## Ready-made example tasks
- [Cybersecurity federal contracts 1m plus](https://apify.com/clearfeedlabs/money-trail-federal-awards/examples/cybersecurity-federal-contracts-1m-plus)
- [Texas nsf hhs grants](https://apify.com/clearfeedlabs/money-trail-federal-awards/examples/texas-nsf-hhs-grants)

## Pricing
Pay per result: **$2.00 per 1,000 awards**, with no subscription. The [Store page](https://apify.com/clearfeedlabs/money-trail-federal-awards) always shows current prices and every optional add-on event.

## FAQ
**Is this data official?** Yes. It comes from the public source named above, and each record links back to it.
**Do I need a login or proxy?** No. It uses documented public endpoints only.
**Can I schedule it?** Yes. Use Apify Schedules, the API or integrations (Zapier, Make, webhooks, MCP-compatible AI agents).

## Links
- Actor on the Apify Store: https://apify.com/clearfeedlabs/money-trail-federal-awards
- Details & pricing: https://clearfeedlabs.com/actors/money-trail-federal-awards/
- Clearfeed Labs: https://clearfeedlabs.com
- Bugs or questions: open an issue on the Actor's Issues tab on Apify.

Data comes from public sources and is provided as-is. Check the original source before relying on it. Not legal, financial or investment advice.

License: MIT
