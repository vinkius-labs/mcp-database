# Leadfeeder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/leadfeeder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Bring Leadfeeder B2B visit intelligence to your AI. Discover which companies visit your website natively.

## Description
Connect your **Leadfeeder** tracking system to an AI agent to analyze high-quality B2B internet traffic. Track precise analytics without using heavy third-party dashboard setups directly in Cursor or Claude.

### What you can do

- **Discover Target Leads:** Fetch the list of verified companies engaging with your tracking pixel on specific domains.
- **Visitor Analytics:** Drill into session specifics of organizations interacting behind the scenes.
- **Sales Pipeline:** Identify key B2B traffic and prioritize new cold email targets or warm follow-ups immediately.

### How it works

1. Install this MCP Server base via Vurb
2. Provide your secure API Developer token
3. Start fetching prospects directly by conversing with your AI

### Who is this for?

- **B2B Sales Reps** — find out today's top visits without leaving the chat pipeline tool
- **Marketing Pros** — verify traffic from latest campaigns instantly by questioning your bot
- **Agency Execs** — extract clean lead directories easily


## Available Tools (9)
- **get_account**: Get details for a specific Leadfeeder account
- **get_custom_feed**: Get details for a specific custom feed filter
- **get_lead**: Get details for a specific lead
- **get_tracking_script**: Get the tracking script for the account
- **list_account_visits**: Get aggregate visits data across the entire account
- **list_accounts**: Retrieve a list of accounts from Leadfeeder
- **list_custom_feeds**: Retrieve the custom feeds active within a specific account
- **list_lead_visits**: Get the website visits directly associated with a specific lead
- **list_leads**: Retrieve a list of discovered leads within an account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Leadfeeder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze and list all identified corporate visitors targeting my site."

**🤖 AI Agent:**
> Connecting to Leadfeeder tracker logs... I've isolated 10 active corporate visits. The principal hit belongs to Microsoft Corp showing interest around the Enterprise Solutions page.

---

**👤 You:**
> "Are there any manufacturing sector companies viewing our price points?"

**🤖 AI Agent:**
> Yes! Filtering by industry: I spot 'Global Steel Corp' navigating the API Pricing tiers specifically on 3 separate occasions today.

---

**👤 You:**
> "Highlight repeat prospects viewing documentation sections."

**🤖 AI Agent:**
> Sorting repeat visitors... Company 'RedHat' holds strong history on the docs segment. They've appeared roughly 14 times spanning the last 2 weeks.


## ❓ FAQ

**Q: How do I authenticate?**
Find your native API Integration string in your web dashboard and pass it as your LEADFEEDER_API_KEY. Our agent queries standard endpoints natively from it.

**Q: Can I filter visitors by country?**
Yes, depending on your prompts, the AI can filter the resulting arrays based on domain and geographical metadata provided.

**Q: How far back does the tracking retention go?**
This mirrors your existing subscription tier limits within the web platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/leadfeeder](https://vinkius.com/mcp/leadfeeder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Leadfeeder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `leadfeeder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Leadfeeder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "leadfeeder": {
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
