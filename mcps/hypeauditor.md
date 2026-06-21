# HypeAuditor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hypeauditor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Analyze influencers and retrieve reports via HypeAuditor API.

## Description
Empower your AI agents with HypeAuditor's industry-leading influencer analytics. This MCP server allows you to search for influencers across Instagram, YouTube, and TikTok, retrieve detailed audit reports, and manage your account insights directly through the HypeAuditor API. Ideal for data-driven influencer marketing and brand protection.


## Available Tools
- **get_account_info**: Gets your HypeAuditor account details
- **get_influencer_report**: Retrieves a detailed report for an influencer
- **get_rate_limit**: Gets current API rate limit status
- **list_categories**: Lists influencer categories
- **list_countries**: Lists available countries
- **list_influencer_types**: Lists available influencer types
- **list_languages**: Lists available languages
- **list_platforms**: Lists supported social media platforms
- **list_reports**: Lists reports generated in your account
- **search_influencers**: Searches for influencers with filters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HypeAuditor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for fashion influencers in France on Instagram."

**🤖 AI Agent:**
> I'll fetch the list of fashion influencers from HypeAuditor for you.

---

**👤 You:**
> "Get an audit report for influencer ID 'xyz-123'."

**🤖 AI Agent:**
> I'll retrieve the detailed audit report for that influencer.

---

**👤 You:**
> "Check my current API rate limit and credits."

**🤖 AI Agent:**
> I'll check your HypeAuditor account status and rate limits.


## ❓ FAQ

**Q: How do I get HypeAuditor API credentials?**
You can find your API token in the HypeAuditor dashboard under 'API Settings'. You may need an enterprise plan to access the API.

**Q: Which platforms are supported?**
The HypeAuditor API supports Instagram, YouTube, and TikTok for influencer search and reporting.

**Q: Can I see my credit balance?**
Yes, the get_account_info tool provides details about your current plan and remaining credits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hypeauditor](https://vinkius.com/mcp/hypeauditor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HypeAuditor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `hypeauditor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HypeAuditor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hypeauditor": {
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
