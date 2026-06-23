# Autobound MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/autobound)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Write hyper-personalized sales emails in seconds using AI that researches prospects and crafts messages that get replies.

## Description
Connect your **Autobound** account to any AI agent and take full control of your outbound sales intelligence and lead enrichment workflows through natural conversation.

### What you can do

- **Signal Orchestration** — Perform high-fidelity semantic search for B2B signals like job changes, funding rounds, and technology adoption using natural language
- **Lead Enrichment Intelligence** — Retrieve real-time buying signals and deep firmographic data for companies and individual contacts using just domains or emails
- **Outbound Content Automation** — Programmatically trigger the generation of highly personalized email and LinkedIn content to coordinate your outreach strategy
- **Campaign Architecture** — Monitor your active outreach campaigns and track lead distribution across your sales funnel to maintain high-fidelity oversight
- **Sales Discovery** — Get a comprehensive overview of prospect activities and buying intent directly through your agent for instant performance reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Autobound dashboard (Settings > API)
3. Start enriching your sales pipeline from Claude, Cursor, or any MCP client

No more manual status checking of individual lead records or digging through complex signal tables. Your AI acts as your dedicated sales analyst and outreach coordinator.

### Who is this for?

- **Sales Development (SDRs)** — instantly build highly targeted lists with deep intent insights using natural language commands
- **Account Executives (AEs)** — monitor buying signals and job changes across key accounts without leaving your workspace
- **Growth Marketers** — automate lead enrichment and personalized content generation through simple AI queries


## Available Tools (12)
- **check_autobound_status**: Verify connectivity
- **enrich_bulk**: Bulk enrich contacts
- **enrich_company**: Enrich a company
- **enrich_contact**: Enrich a contact
- **execute_campaign**: Execute a campaign
- **generate_email**: Generate sales email
- **generate_linkedin**: Generate LinkedIn message
- **get_campaign**: Get campaign details
- **get_signal**: Get signal details
- **list_campaigns**: List campaigns
- **list_prospects**: List prospects
- **search_signals**: Search buyer signals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Autobound** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for companies in New York with a recent 'Funding' signal."

**🤖 AI Agent:**
> I've performed the semantic search. I found 8 companies in New York with active funding signals, including 'TechFlow' (Series B) and 'GreenGrid'. Would you like the detailed high-fidelity metadata for any of these?

---

**👤 You:**
> "Enrich domain 'vinkius.com' and show buying signals."

**🤖 AI Agent:**
> Enrichment complete! For vinkius.com, I've identified 3 high-fidelity signals: a new 'Head of Engineering' hire and 2 tech adoption updates. Shall I generate a personalized outreach email based on these?

---

**👤 You:**
> "List all active outbound campaigns in my Autobound account."

**🤖 AI Agent:**
> Accessing campaign architecture... You have 5 active campaigns, including 'Q2 Tech Founders' and 'AI Outreach'. Lead volume is trending up in your top funnel. Would you like the detailed performance metadata?


## ❓ FAQ

**Q: How do I find my Autobound API Key?**
Log in to your account, navigate to **Settings** > **API**, and copy your unique secret key.

**Q: What counts as a buying signal?**
Autobound tracks semantic events like executive job changes, funding milestones, or the deployment of new technologies in a company's stack.

**Q: Can I enrich multiple domains at once?**
The current toolset is optimized for granular, high-fidelity enrichment of individual domains and emails to ensure accurate signal discovery.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/autobound](https://vinkius.com/mcp/autobound)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Autobound** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `autobound` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Autobound** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "autobound": {
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
