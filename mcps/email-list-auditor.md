# Email List Auditor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/email-list-auditor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Analyze email subscriber counts, health scores, and list composition.

## Description
This MCP server provides tools to audit and analyze email subscription lists. You can use `get_total_subscriber_count` to find the total size of a list, `get_subscriber_status_breakdown` to see the ratio of active to inactive users, and `calculate_list_health_score` to determine if a list is ready for a campaign. It also includes `list_subscribers_by_tier` to segment lists into Small, Medium, or Large categories.


## Available Tools (4)
- **calculate_list_health_score**: Calculate the health score of an email list
- **get_subscriber_status_breakdown**: Get the breakdown of subscriber statuses in a list
- **get_total_subscriber_count**: Get the total number of subscribers in a specific list
- **list_subscribers_by_tier**: List subscriber counts by size tier


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Email List Auditor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many total subscribers are in list ID 12345?"

**🤖 AI Agent:**
> There are 5,000 total subscribers in list 12345.

---

**👤 You:**
> "What is the health status of list 98765?"

**🤖 AI Agent:**
> The health score for list 98765 is 85%, which is rated as 'Healthy'.

---

**👤 You:**
> "Give me the status breakdown for list 55555."

**🤖 AI Agent:**
> For list 55555, there are 450 subscribed users, 40 unsubscribed users, and 10 bounced users.


## ❓ FAQ

**Q: How can I check if my email list is healthy?**
You can use the `calculate_list_health_score` tool to get a percentage and a qualitative status like 'Healthy' or 'At Risk'.

**Q: What information is included in the status breakdown?**
The `get_subscriber_status_breakdown` tool provides the count of users with 'Subscribed', 'Unsubscribed', and 'Bounced' statuses.

**Q: Can I see how many subscribers are in different size tiers?**
Yes, the `list_subscribers_by_tier` tool categorizes subscribers into Small, Medium, and Large tiers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/email-list-auditor](https://vinkius.com/en/ai-agent-connect/email-list-auditor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Email List Auditor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `email-list-auditor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Email List Auditor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "email-list-auditor": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
