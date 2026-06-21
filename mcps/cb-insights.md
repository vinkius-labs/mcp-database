# CB Insights MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cb-insights)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Research emerging technologies, track venture capital deals, and analyze market trends with AI-powered business intelligence.

## Description
Connect your **CB Insights** enterprise account to any AI agent and take full control of your market intelligence workflows through natural conversation.

### What you can do

- **Organization Research** — Search companies by name and retrieve full profiles including industry classification, employee count, and headquarters
- **Funding Intelligence** — Track the complete funding history of any organization, from Seed rounds to IPO, with amounts and lead investors
- **Competitive Mapping** — Identify direct competitors for any company based on market positioning and funding patterns
- **Deal Tracking** — Browse recent investment deals across the market or filter by specific organizations
- **Investor Profiling** — Explore investor profiles, fund strategies, and their full portfolio of backed companies
- **AI-Powered Q&A** — Ask natural language questions about markets, trends, and technologies and get data-backed answers

### How it works

1. Subscribe to this server
2. Enter your CB Insights Client ID and Client Secret (provisioned by your account manager)
3. Start querying market intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Venture Capitalists** — instantly screen deal flow, check competitor landscapes, and validate funding histories without switching tools
- **Corporate Strategy Teams** — monitor market movements, track emerging competitors, and assess investment opportunities through conversational AI
- **Founders & Entrepreneurs** — research investors, understand competitive dynamics, and prepare for fundraising rounds with comprehensive data


## Available Tools
- **chat_cbi**: CB Insights AI chat
- **check_cbi_status**: Verify connectivity
- **get_deal**: Get deal details
- **get_investor**: Get investor details
- **get_org_competitors**: Get competitors
- **get_org_funding**: Get organization funding
- **get_organization**: Get organization details
- **get_investor_portfolio**: Get investor portfolio
- **list_deals_by_org**: List deals by organization
- **list_deals**: List recent deals
- **list_industries**: List industries
- **list_investors**: List investors
- **list_organizations**: Search organizations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CB Insights** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the company OpenAI and show me its full funding history."

**🤖 AI Agent:**
> I found OpenAI (Org ID: org_38291). Running the funding query... OpenAI has raised $11.3B across 7 rounds. The latest was a $6.6B Series B led by Thrive Capital in October 2024. Earlier rounds include a $300M Series A from Microsoft. Would you like me to list its competitors?

---

**👤 You:**
> "Who are the top competitors of Anthropic in the AI space?"

**🤖 AI Agent:**
> Searching for Anthropic... Found Org ID: org_44102. Running competitive analysis... The top 5 competitors by market overlap are: OpenAI (highest funding match), Cohere, AI21 Labs, Mistral AI, and Inflection AI. OpenAI leads with $11.3B raised vs Anthropic's $7.3B. Would you like investor details for any of these?

---

**👤 You:**
> "Show me the full portfolio of Sequoia Capital and highlight their AI investments."

**🤖 AI Agent:**
> Fetching Sequoia Capital's profile (Investor ID: inv_9021)... Their portfolio contains 412 active companies. Notable AI-focused investments include: Anthropic ($700M), Scale AI ($325M), and Hugging Face ($235M). The median check size across their portfolio is $28M at Series B stage. Would you like to see deal details for any of these companies?


## ❓ FAQ

**Q: Can my AI agent retrieve the full funding history of a specific company just by providing the Organization ID?**
Yes! Use the `get_org_funding` tool with the Organization ID. Your agent will return every funding round — Seed, Series A through D, and IPO — including amounts raised, lead investors, round dates, and post-money valuations.

**Q: How do I map out the competitive landscape for a target company?**
Simply ask the agent to run `get_org_competitors` with the Organization ID. It will return direct competitors ranked by market positioning, funding similarity, and industry overlap, giving you an instant competitive analysis.

**Q: Does the integration allow modifying data or creating entries in CB Insights?**
No. All 13 tools are strictly read-only query operations — searching organizations, tracking funding, analyzing competitors, and exploring investors. The only write operation is `chat_cbi`, which sends a question to the AI engine. No destructive actions exist, ensuring your data remains secure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cb-insights](https://vinkius.com/mcp/cb-insights)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CB Insights** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `cb-insights` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CB Insights** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cb-insights": {
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
