# Jebbit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jebbit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Access interactive experiences and zero-party data via Jebbit API.

## Description
Empower your AI agents with Jebbit's interactive experience platform. This MCP server allows you to list experiences, retrieve consumer attributes, manage audience segments, and track reporting jobs directly through the Jebbit API. Ideal for leveraging zero-party data and automating marketing insights.


## Available Tools (10)
- **get_account**: Use to verify account status.

Retrieves account details
- **list_attributes**: g., "favorite_color", "purchase_intent") that have been captured across experiences. Essential for understanding what consumer insights are available.

Lists all consumer attributes captured
- **get_experience**: Use this to understand the structure or overall results of a specific quiz or survey.

Retrieves details for a specific experience
- **list_campaigns**: Use this to monitor where traffic to experiences is coming from.

Lists all active campaigns
- **list_experiences**: Returns experience names, IDs, and publication status. Use this to identify which interactive content is available for analysis.

Lists all interactive experiences
- **list_integrations**: Useful for verifying data flow to other platforms.

Lists all active integrations
- **list_reporting_jobs**: Use this to check the status of large data requests.

Lists all recent reporting jobs
- **list_segments**: Useful for identifying high-value cohorts for targeted marketing.

Lists all audience segments
- **list_users**: Useful for account auditing and permission checks.

Lists all platform users
- **list_webhooks**: Useful for auditing integrations.

Lists all configured webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jebbit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all interactive experiences in my Jebbit account."

**🤖 AI Agent:**
> I'll fetch the list of your active Jebbit experiences for you.

---

**👤 You:**
> "Show me the consumer attributes captured by my quizzes."

**🤖 AI Agent:**
> I'll retrieve the list of attributes and zero-party data points from Jebbit.

---

**👤 You:**
> "Check for any recent reporting jobs."

**🤖 AI Agent:**
> I'll look up the status of your recent data reporting jobs in Jebbit.


## ❓ FAQ

**Q: How do I get Jebbit API credentials?**
You need a Client ID and Client Secret. Please contact your Jebbit account representative or visit the developer settings in your Jebbit dashboard to obtain these credentials.

**Q: What is zero-party data?**
Zero-party data is data that a customer intentionally and proactively shares with a brand, often through interactive experiences like quizzes or surveys.

**Q: Can I see campaign performance?**
Yes, the list_reporting_jobs and get_experience tools allow you to access data related to how users are interacting with your Jebbit content.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jebbit](https://vinkius.com/mcp/jebbit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Jebbit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jebbit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Jebbit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jebbit": {
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
