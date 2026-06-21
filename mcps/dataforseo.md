# DataForSEO MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dataforseo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage SERP data via DataForSEO — track Google organic rankings, audit Maps nodes, monitor News publications, and research Amazon products directly from any AI agent.

## Description
Connect your **DataForSEO** account to any AI agent and take full control of your search engine marketing and data research workflows through natural conversation.

### What you can do

- **Organic SERP Auditing** — List 100+ deep positional stats for Google, Bing, Yahoo, Yandex, and Baidu to identify topical authority and ranking limits
- **Google Maps Navigation** — Analyze local GMB 3-pack nodes down to exact GPS review coordinates and verify local business discoverability
- **Real-Time News Monitoring** — Retrieve explicitly fresh PR and syndicated publication stamps from Google News, bypassing standard cache strictly
- **Visual Search Discovery** — Index purely visual array vectors matching exact keywords from Google Images to monitor brand visual footprints
- **Amazon Retail Insights** — Capture live Price, BSR (Best Sellers Rank), and Prime Stock variables natively by ASIN to audit e-commerce competition
- **Geographic Precision** — Specify exact map location strings (e.g., 'London, England') to retrieve localized search results and regional ranking differentials

### How it works

1. Subscribe to this server
2. Enter your DataForSEO API Login and API Password (found in the API Access section of your Dashboard)
3. Start researching SERP data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SEO Specialists** — monitor organic rankings and perform deep competitor analysis without manual search exports
- **Local Marketers** — audit Google Maps visibility and GMB positioning for specific geographic locations
- **E-commerce Managers** — track Amazon product prices and Best Sellers Rank using natural language
- **Data Analysts** — retrieve structured SERP data across multiple search engines for market research and trend analysis


## Available Tools (10)
- **amazon_asin**: Identify precise active arrays spanning native Hold parsing
- **baidu_organic**: ` parsing CN exact local search features excluding un-indexed subsets.

Identify precise active arrays spanning native Gateway auth
- **bing_organic**: ` tracking Microsoft Graph differentials against the main Google DB natively.

Irreversibly vaporize explicit validations extracting rich Churn flags
- **google_organic**: Identify bounded CRM records inside the Headless DataForSEO Platform
- **google_images**: Retrieve explicit Cloud logging tracing explicit Vault limits
- **google_maps**: Perform structural extraction of properties driving active Account logic
- **google_news**: Provision a highly-available JSON Payload generating hard Customer bindings
- **yahoo_organic**: ` identifying Legacy SERP positions across regional domains specifically.

Enumerate explicitly attached structured rules exporting active Billing
- **yandex_organic**: ` resolving top ranking CIS regional indexes fully decoupled from western rules.

Dispatch an automated validation check routing explicit Gateway history
- **youtube_organic**: ` returning direct streaming video rankings and exact metadata counts.

Inspect deep internal arrays mitigating specific Plan Math


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DataForSEO** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get Google organic results for 'best CRM software' in the United States"

**🤖 AI Agent:**
> Retrieving Google SERP data for the US... I found the top 100 organic results. Ranking #1 is 'Salesforce', followed by 'HubSpot' and 'Zendesk'. I can provide the rich snippets and estimated traffic for these links.

---

**👤 You:**
> "Show me the top 3 businesses on Google Maps for 'Italian Restaurant' in London"

**🤖 AI Agent:**
> Analyzing London GMB results... The top 3 Italian restaurants are 'Bella Italia', 'Padella', and 'Trullo'. I have their GPS coordinates, review counts, and average ratings available.

---

**👤 You:**
> "Get Amazon price and BSR for ASIN 'B08N5KWB9H' in the UK"

**🤖 AI Agent:**
> Retrieving Amazon UK data for ASIN B08N5KWB9H... Current Price: £899.00, Best Sellers Rank: #1 in Electronics. Prime shipping is available. Would you like to track historical price changes?


## ❓ FAQ

**Q: Can my agent retrieve localized Google search results for a specific city?**
Yes. Provide the city or country name in the 'location' parameter. The agent will query DataForSEO's localized endpoints to return the exact SERP results as seen by users in that specific geographic boundary.

**Q: How do I audit competitor rankings across different search engines?**
You can use specialized tools for each engine (google_organic, bing_organic, baidu_organic, etc.). Provide the target keyword, and the agent will retrieve the top positional stats, allowing you to compare rankings across multiple global indexes.

**Q: Does the agent help with Amazon product price and stock monitoring?**
Absolutely. The 'amazon_asin' tool retrieves live retail data including Price, Best Sellers Rank (BSR), and Prime availability. Your agent can track these variables natively by ASIN to monitor e-commerce trends.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dataforseo](https://vinkius.com/mcp/dataforseo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DataForSEO** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dataforseo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DataForSEO** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dataforseo": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
