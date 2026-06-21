# Harmonic MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/harmonic)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Automate company and startup intelligence via Harmonic — enrich domains, track funding, and discover investors directly from any AI agent.

## Description
Connect your **Harmonic.ai** account to any AI agent and take full control of your startup discovery and investment research through natural conversation.

### What you can do

- **Company Enrichment** — Instantly retrieve firmographics, funding history, and social traction signals for any domain.
- **Person Insights** — Enrich professional profiles using LinkedIn URLs to get education and career history.
- **Startup Discovery** — Search through over 35 million companies using advanced filters like headcount growth and industry.
- **Investor Research** — Find investment firms and angels, and inspect their full portfolio history.
- **Funding Monitoring** — List and retrieve details for funding rounds, including amounts and lead investors.
- **Enrichment Status** — Track background data refresh requests to ensure you have the most up-to-date information.

### How it works

1. Subscribe to this server
2. Enter your Harmonic API Key (found in the Console)
3. Start discovering startups from Claude, Cursor, or any MCP-compatible client

No more manual exporting of company lists. Your AI assistant acts as a dedicated Venture Analyst or Market Research Associate.

### Who is this for?

- **Venture Capitalists** — instantly retrieve a startup's funding history and team signals during deal sourcing.
- **Sales Teams** — automate the enrichment of target accounts and identify high-growth companies.
- **Corporate Devs** — maintain a real-time overview of competitor funding and acquisition targets.


## Available Tools
- **enrich_company**: Enrich a company with firmographics, funding, and social signals
- **enrich_person**: Enrich a person with professional history and social signals
- **get_company_stats**: Get growth and headcount statistics for a company
- **get_enrichment_status**: Check the status of a background enrichment request
- **get_investor_portfolio**: Get the list of portfolio companies for an investor
- **get_api_profile**: Get information about the current API user
- **list_company_news**: List recent news and press releases for a company
- **list_funding_rounds**: List funding rounds for a specific company
- **list_traction_signals**: List social and web traction signals for a company
- **search_investors**: Search for investment firms and angels
- **search_startups**: Search for startups using filters like industry, location, and headcount


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Harmonic** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Enrich the domain 'openai.com' and show funding rounds."

**🤖 AI Agent:**
> Accessing Harmonic data... OpenAI has raised significant funding from investors like Microsoft and Sequoia. Their latest round was a Corporate Round in 2024. Would you like to see the full list of individual funding events?

---

**👤 You:**
> "Search for startups in 'Artificial Intelligence' with 50-200 employees."

**🤖 AI Agent:**
> Searching database... I found 12 companies matching your criteria, including 'Anthropic', 'Cohere', and 'Mistral AI'. Should I retrieve the traction signals for the top 3 results?

---

**👤 You:**
> "Show me the portfolio companies for 'Sequoia Capital'."

**🤖 AI Agent:**
> Retrieving portfolio... Sequoia Capital has invested in over 1,500 companies, including giants like Apple, Google, and Stripe. Recently, they've been active in the AI sector with investments in 'Harvey' and 'Glean'. Would you like more details on their recent AI deals?


## ❓ FAQ

**Q: How do I find my Harmonic API Key?**
Log in to your Harmonic account, go to the **Console**, and navigate to the **API** section. You will be able to generate and copy your unique apikey from there.

**Q: What happens if a company is not found in the database?**
If a company is not found, Harmonic will return a `201 Enrichment Triggered` status. This means a background update has been queued. You can check the status later using the `get_enrichment_status` tool.

**Q: Can I search for companies based on specific criteria?**
Yes! Use the `search_startups` tool. You can provide a JSON string with filters like headcount, location, or industry to find companies that match your investment or sales criteria.

**Q: Is the integration secure?**
Absolutely. The integration only accesses your data through your unique API key. Your credentials are encrypted and stored securely within the Vinkius Cloud infrastructure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/harmonic](https://vinkius.com/mcp/harmonic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Harmonic** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `harmonic` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Harmonic** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "harmonic": {
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
