# UK Planning Applications Scraper – 400+ Councils & Postcodes

Export UK planning applications from 400+ councils by keyword, council, or postcode radius: address, description, status, dates, coordinates and documents link. Powered by the PlanIt open API. Pay per result.

**[Run it on Apify →](https://apify.com/devteamdrew/uk-planning-applications?utm_source=github&utm_medium=readme&utm_campaign=uk-planning-applications)** (pay per result, free Apify account to start)


**UK Planning Applications Scraper** by Moxie: fast, reliable and polite, built on official/public data sources.

## What can it do?

- Lead generation for builders, architects, solar and EV-charger installers
- Property development and land intelligence
- Monitoring a postcode or council for new applications (incremental mode)
- Market research on extensions, HMOs, change of use

## Data source

PlanIt (planit.org.uk), an open aggregator of UK council planning portals. Public data only.

## Features

- **Pay only for results** (pay-per-event pricing, no monthly rental)
- **Incremental mode**: scheduled runs return only items you haven't received before
- **LLM-ready output**: optional compact Markdown per item for RAG / AI agents
- **Polite rate limiting** with automatic retries and backoff
- Clean, flat JSON you can export as CSV, Excel, JSON or via API


## Quick start

1. Create a free account at [apify.com](https://apify.com/devteamdrew/uk-planning-applications?utm_source=github&utm_medium=readme&utm_campaign=uk-planning-applications) and copy your API token.
2. `export APIFY_TOKEN=...`
3. Run one of the examples:

```bash
bash examples/run.sh          # curl
node examples/run.js          # JavaScript (apify-client)
python examples/run.py        # Python (apify-client)
```

Example input ([examples/input.json](examples/input.json)):

```json
{
  "search": "solar",
  "recentDays": 30,
  "maxItems": 20,
  "includeDetails": true
}
```

## Use with AI agents (MCP)

Add `https://mcp.apify.com/?actors=devteamdrew/uk-planning-applications` as an MCP server in Claude, Cursor or any MCP client.

## Pricing

See the [Apify Store page](https://apify.com/devteamdrew/uk-planning-applications?utm_source=github&utm_medium=readme&utm_campaign=uk-planning-applications) for current pay-per-result pricing.

## More data actors

- [Bluesky Scraper & API – Posts, Profiles & Search](https://apify.com/devteamdrew/bluesky-scraper?utm_source=github&utm_medium=readme&utm_campaign=uk-planning-applications)
- [Companies House Scraper – UK Company Data, Directors & Filings](https://apify.com/devteamdrew/companies-house-scraper?utm_source=github&utm_medium=readme&utm_campaign=uk-planning-applications)
- [Hacker News Scraper – Stories, Comments & Who Is Hiring Jobs](https://apify.com/devteamdrew/hacker-news-scraper?utm_source=github&utm_medium=readme&utm_campaign=uk-planning-applications)
- [npm Scraper – Package Downloads, Dependencies & Maintainers](https://apify.com/devteamdrew/npm-package-scraper?utm_source=github&utm_medium=readme&utm_campaign=uk-planning-applications)
- [GitHub Trending Scraper – Repos, Stars & Developers](https://apify.com/devteamdrew/github-trending-scraper?utm_source=github&utm_medium=readme&utm_campaign=uk-planning-applications)
- [Mastodon Scraper – Fediverse Hashtags, Accounts & Trends](https://apify.com/devteamdrew/mastodon-scraper?utm_source=github&utm_medium=readme&utm_campaign=uk-planning-applications)
- [Lemmy Scraper – Posts, Comments & Communities (Fediverse)](https://apify.com/devteamdrew/lemmy-scraper?utm_source=github&utm_medium=readme&utm_campaign=uk-planning-applications)

## License

Examples in this repository are MIT licensed. The actor itself runs on the Apify platform.
