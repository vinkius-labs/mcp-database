# Crunchbase MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crunchbase)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

AI business intelligence: search companies, track funding, and analyze investments via agents.

## Description
### What you can do

Connect AI agents to the Crunchbase API for comprehensive business intelligence and startup ecosystem analysis:

- **Search companies** by name to find startups, enterprises, and emerging tech firms
- **Get complete company profiles** with founding dates, headquarters, employee counts, and operating status
- **Track funding rounds** from Seed to Series D+ with amounts, dates, and investor syndicates
- **Analyze acquisition history** to understand M&A strategies and consolidation patterns
- **Research investors** including VC firms, angels, and corporate venture arms with full portfolios
- **Find entrepreneurs and executives** with detailed career histories and board memberships
- **Monitor IPO activity** with stock exchange details, ticker symbols, and offering data
- **Map investment networks** to identify co-investor relationships and deal flow patterns

### How it works

1. **Get your Crunchbase API key** from data.crunchbase.com (requires paid license)
2. **Ask your AI agent** to research companies, analyze funding trends, or map investor networks
3. **Natural language commands** replace manual Crunchbase website searches
4. **Structured business data** returned in formatted responses for quick analysis

### Who is this for?

Essential for **venture capitalists**, **startup founders**, **business development professionals**, **market researchers**, **investment bankers**, **corporate strategists**, and **journalists**. Let AI agents perform company due diligence, track competitor funding activity, identify potential acquisition targets, research investor backgrounds, and map ecosystem relationships. Perfect for professionals who need to answer questions like 'Who invested in Stripe's Series B?', 'What companies has Google acquired since 2020?', or 'Which VCs are most active in AI/ML startups?'


## Available Tools
- **get_acquisition_details**: Use this after list_acquisitions to understand the full context of a specific M&A deal.

Get complete details of a specific acquisition transaction
- **get_funding_round_details**: ), announced date, all participating investors with their investment roles (lead, participant), pre-money and post-money valuations if disclosed, number of investors, and associated press release links. Use this after list_funding_rounds to deep-dive into a specific funding event.

Get detailed information about a specific funding round transaction
- **get_ipo_details**: ), ticker symbol, IPO date, share price at offering, number of shares offered, total capital raised from IPO, and post-IPO valuation. Use this for companies that have gone public to understand their transition from private to public markets.

Get IPO (Initial Public Offering) details for a public organization
- **get_organization_details**: Returns the entity overview with all known metadata Crunchbase has on file. Use this after search_organizations to get the full company profile including funding totals, acquisition history, and key personnel.

Get complete profile and metadata for a specific organization from Crunchbase
- **get_person_details**: Use this after search_people to get the full biography and career history of founders, investors, or executives.

Get detailed professional profile for a specific person from Crunchbase
- **list_acquisitions**: Shows companies acquired by this organization (if it's an acquirer) or acquisition events where this organization was the target. Each acquisition includes the acquired company name, acquisition date, price (if disclosed), acquisition type (acquisition, merger, acquihire, buyout), and acquiring company details. Use this to understand a company's growth-through-acquisition strategy or identify which companies a startup has absorbed.

List all acquisitions made by or involving a specific organization
- **list_funding_rounds**: Each funding round includes the stage (Seed, Angel, Series A, Series B, Series C, Series D+, Series Unknown, Convertible Note, Post-IPO Equity, Post-IPO Debt, Grant, Venture Round, Corporate Round), announced date, amount raised (in USD if available), lead investors, participating investors, and post-money valuation if disclosed. Use this to analyze a company's fundraising trajectory, total capital raised, and investor syndicate.

List all funding rounds (Seed, Series A/B/C, IPO, etc.) for a specific organization
- **list_investments**: Each investment entry includes the company invested in, funding round participated (Seed, Series A, etc.), investment date, co-investors in the same round, and whether this investor led the round. Use this to analyze a VC firm's investment thesis, portfolio diversity, recent deal activity, or find startups backed by a specific investor.

List all investments made by a specific organization or investor
- **search_organizations**: Returns organization names, short descriptions, operational status (operating, acquired, closed), headquarters locations, and industry categories. Use this as the first step to find a company before getting detailed funding, acquisition, or personnel data. The search returns up to 20 matching organizations ranked by relevance.

Search for companies and organizations by name keyword in Crunchbase
- **search_people**: Returns person names, current job titles, organizational affiliations, locations, and brief career summaries. Use this to find founders, CEOs, investors, or board members before getting their detailed profiles with investment history and professional relationships.

Search for entrepreneurs, investors, executives, and board members by name in Crunchbase


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crunchbase** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all funding rounds raised by Stripe and show me the total amount raised"

**🤖 AI Agent:**
> I'll find Stripe and pull their complete funding history with amounts and investors.

---

**👤 You:**
> "Which venture capital firms invested in OpenAI's funding rounds?"

**🤖 AI Agent:**
> I'll get OpenAI's funding rounds and extract all participating VC firms.

---

**👤 You:**
> "Show me all companies acquired by Google in the last 5 years"

**🤖 AI Agent:**
> I'll pull Google's acquisition history with dates, prices, and acquired company details.


## ❓ FAQ

**Q: Do I need a paid Crunchbase license to use this MCP?**
Yes, the Crunchbase API requires a paid license (Starter, Professional, or Enterprise tier). Free accounts have limited access. Your API key (user_key) is provided via email upon license activation. Contact Crunchbase sales at data@crunchbase.com for licensing options.

**Q: Can I track real-time funding announcements and new startup launches?**
Crunchbase data is updated regularly but not in real-time. Funding rounds appear within days of public announcement. The API provides the most recent data Crunchbase has processed. For real-time monitoring, consider combining this MCP with news API monitoring for immediate PR detection.

**Q: Can I search for companies by industry or location instead of name?**
This MCP currently supports name-based search. For industry/location filtering, you can search with broad terms and then review company profiles for location and industry details in the detailed results. Advanced filtering by industry vertical, funding stage, or employee count would require the Crunchbase Enterprise API tier with additional query capabilities.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crunchbase](https://vinkius.com/mcp/crunchbase)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Crunchbase** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `crunchbase` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Crunchbase** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crunchbase": {
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
