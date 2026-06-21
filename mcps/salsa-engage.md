# Salsa Engage MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/salsa-engage)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate non-profit outreach via Salsa Engage — manage supporters, activities, and fundraising analytics with AI.

## Description
Connect your **Salsa Engage** account to any AI agent and take full control of your non-profit outreach and supporter orchestration through natural conversation. Salsa Engage provides a comprehensive platform for fundraising, advocacy, and marketing automation, and this integration allows you to retrieve supporter metadata, monitor engagement activities, and manage groups directly from your chat interface.

### What you can do

- **Supporter & Donor Orchestration** — List all managed supporters and retrieve detailed profile metadata, including upserting contact records programmatically.
- **Engagement Activity Intelligence** — Access and monitor signatures, form submissions, and fundraising data to maintain a clear overview of campaign progress directly from the AI interface.
- **Group & Segment Control** — Manage supporter groups and assign contacts to targeted lists to ensure your communication is always synchronized via natural language.
- **Operational Monitoring** — Track system metrics, monitor webhooks, and retrieve account profile metadata using simple AI commands.
- **Offline Donation Oversight** — Access and list offline donation records to keep your financial and engagement data consistent.

### How it works

1. Subscribe to this server
2. Enter your Salsa Engage API Token from your organization settings
3. Start managing your engagement workflows from Claude, Cursor, or any MCP-compatible client

No more manual report exports or group syncing. Your AI acts as a dedicated engagement coordinator or advocacy lead.

### Who is this for?

- **Non-profit Organizers** — quickly retrieve supporter details and monitor petition counts without switching apps.
- **Digital Marketers** — automate the management of targeted groups and track activity metrics via natural conversation.
- **Advocacy Teams** — streamline the retrieval of engagement data and monitor campaign health directly within the chat.


## Available Tools
- **assign_supporters_to_group**: Add supporters to a group
- **check_api_health**: Verify Salsa Engage API connectivity
- **get_account_info**: Get authenticated account details
- **get_engagement_metrics**: Retrieve performance metrics
- **list_engagement_activities**: Search and list activities
- **list_offline_donations**: List offline donation records
- **list_supporter_groups**: Search and list groups
- **list_supporter_segments**: List defined segments
- **list_supporters**: Search and list supporters
- **list_configured_webhooks**: List active webhooks
- **upsert_supporter_group**: Create or update a group
- **upsert_supporter_profile**: Create or update a supporter


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salsa Engage** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active supporter groups in Salsa Engage."

**🤖 AI Agent:**
> I've retrieved your groups. You have 5 active segments including 'Monthly Donors', 'Advocacy Leads', and 'New Volunteers'. Which one would you like to assign supporters to?

---

**👤 You:**
> "Show me all active donor campaigns with their fundraising progress and goal completion rates."

**🤖 AI Agent:**
> 7 active fundraising campaigns. "Annual Fund 2025" raised $234,000 of $500,000 goal (46.8%). "Spring Gala" at $89,000 of $100,000 (89%, on track). "Building Expansion" at $1.2M of $5M (24%, major gift pending). "Scholarship Fund" at $67,000 of $150,000 (44.7%). "Emergency Relief" at $34,000 of $50,000 (68%). "Youth Programs" at $23,000 of $75,000 (30.7%). "Endowment" at $890K of $2M (44.5%). Total donors this quarter: 2,340. Average gift: $127. Retention rate: 72%.

---

**👤 You:**
> "List all major donors who have given more than $5,000 this year and their giving history."

**🤖 AI Agent:**
> 34 major donors ($5,000+) this year. Top 5: Robert Chen ($50,000, 8-year donor), Sarah Williams ($25,000, monthly recurring), James Park ($18,000, first-time major), Lisa Wang ($15,000, board member), David Kim ($12,000, event sponsor). Total major gifts: $456,000. Average major gift: $13,412. 12 donors upgraded from mid-level. 5 are legacy society members. 8 have pending pledges. Recommended cultivation: 6 donors near $10K threshold for next recognition level.


## ❓ FAQ

**Q: Can my AI automatically find all supporters who signed a specific petition today?**
Yes! Use the `list_engagement_activities` tool with a date filter. Your agent will respond with the complete metadata for all participants and their submission details in seconds.

**Q: How do I find my Salsa Engage API Token?**
Log in to your Salsa Engage account, navigate to **Organization Settings** > **API** tab, and you will find your unique Integration API token listed there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/salsa-engage](https://vinkius.com/mcp/salsa-engage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Salsa Engage** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `salsa-engage` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Salsa Engage** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "salsa-engage": {
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
