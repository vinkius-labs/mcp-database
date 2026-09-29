# Membership Records Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/membership-records-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [compliance](../categories/compliance.md)

Manage membership lifecycles, renewal calendars, and compliance checklists.

## Description
This MCP server provides administrative tools to manage the full membership lifecycle. It allows users to generate consolidated membership registers using `get_membership_register`, identify upcoming deadlines with `get_renewal_calendar`, create personalized termination requirements via `get_cancellation_checklist`, and define audit duties through `get_annual_review_tasks`. It is designed to handle renewal lead times, benefit evidence verification, and authorized user access rules.


## Available Tools (4)
- **get_renewal_calendar**: Identify upcoming renewal deadlines
- **get_annual_review_tasks**: Define administrative duties required to audit membership accuracy and benefit alignment
- **get_cancellation_checklist**: Generate a personalized list of requirements for terminating a specific membership
- **get_membership_register**: Provide a consolidated list of all active and pending memberships


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Membership Records Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me a list of all my current memberships."

**🤖 AI Agent:**
> Here is the consolidated list of your active and pending memberships.

---

**👤 You:**
> "Which memberships are due for renewal in the next 30 days?"

**🤖 AI Agent:**
> The following memberships require attention within the next 30 days: John Doe (Expires Oct 15) and Jane Smith (Expires Oct 28).

---

**👤 You:**
> "What do I need to do to cancel member ID 12345?"

**🤖 AI Agent:**
> To cancel this membership, you must: Return physical card, Submit final receipt, and Confirm authorized user removal.


## ❓ FAQ

**Q: How can I see all my active memberships?**
You can use the `get_membership_register` tool to receive a consolidated list of all active and pending memberships.

**Q: How do I prepare for a membership expiration?**
Use the `get_renewal_calendar` tool to identify upcoming deadlines based on your preferred renewal lead time.

**Q: What is needed to cancel a membership?**
The `get_cancellation_checklist` tool generates a personalized list of tasks and documents required for termination based on the specific member's benefits and storage preferences.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/membership-records-plan](https://vinkius.com/en/ai-agent-connect/membership-records-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Membership Records Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `membership-records-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Membership Records Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "membership-records-plan": {
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
