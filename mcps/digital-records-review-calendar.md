# Digital Records Review Calendar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/digital-records-review-calendar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transform record governance policies into actionable review schedules.

## Description
This MCP server connects AI agents to your digital record governance system. It allows agents to manage compliance by using tools like `list_record_groups` to identify managed assets, `calculate_review_schedule` to map out upcoming audit windows, `get_group_retention_details` to retrieve legal destruction mandates, and `get_reminder_notifications` to plan owner alerts. It bridges the gap between static policy and active scheduling.


## Available Tools (4)
- **get_group_retention_details**: Get specific retention and destruction rules for a group
- **get_reminder_notifications**: Get the upcoming reminder notification details
- **list_record_groups**: List all managed record groups
- **calculate_review_schedule**: Calculate upcoming review events within a date range


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Digital Records Review Calendar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What record groups are currently managed in the system?"

**🤖 AI Agent:**
> The system currently manages the following record groups: Financial Audits 2023, Employee Onboarding, and Legal Contracts.

---

**👤 You:**
> "When is the next review for the Financial Audits 2023 group?"

**🤖 AI Agent:**
> The next review for Financial Audits 2023 is scheduled for October 15th, 2024.

---

**👤 You:**
> "What are the retention rules for the Employee Onboarding group?"

**🤖 AI Agent:**
> The Employee Onboarding group must be kept for 7 years, after which the destruction action is Digital Shredding.


## ❓ FAQ

**Q: How can I see all my managed record groups?**
You can use the `list_record_groups` tool to retrieve a list of all managed groups, including their owners and next review dates.

**Q: How do I find out when a specific review is due?**
Use the `calculate_review_schedule` tool with a specific date range to find all upcoming review events.

**Q: Can I check the retention rules for a specific group?**
Yes, the `get_group_retention_details` tool provides the specific legal and operational mandates for any given group ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/digital-records-review-calendar](https://vinkius.com/en/ai-agent-connect/digital-records-review-calendar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Digital Records Review Calendar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `digital-records-review-calendar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Digital Records Review Calendar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "digital-records-review-calendar": {
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
