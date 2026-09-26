# Household Safety Drill Record MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/household-safety-drill-record)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Document and audit residential emergency preparedness drills.

## Description
This MCP server provides a structured way to manage residential emergency preparedness. Use `record_drill_session` to capture drill data, `get_drill_summary` for high-level overviews, and `verify_drill_readiness` to check if remediation is complete. It also includes `list_action_items` to track all pending safety fixes across your household drills.


## Available Tools (4)
- **get_drill_summary**: Provides a high-level overview of a specific drill's outcomes and pending tasks
- **list_action_items**: You can optionally filter by status.

Retrieves all unresolved issues and fixes across all drills that require immediate attention
- **record_drill_session**: Ensure drillDate and reviewDate are provided.

Captures the raw data from a completed household safety exercise to create a formal record
- **verify_drill_readiness**: Determines if a drill record is "follow-up-ready" based on whether the review date has passed and fixes are addressed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Household Safety Drill Record** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I just finished a safety drill. We practiced the hallway exit on 2023-10-15. Participants were Alice and Bob. The meeting point is the front gate. We noticed the back door was stuck. We decided to oil the hinges. We will review this on 2023-10-20."

**🤖 AI Agent:**
> The drill session has been recorded. Status is set to Action Required due to the stuck back door.

---

**👤 You:**
> "Can you give me a summary of drill ID 12345?"

**🤖 AI Agent:**
> Drill 12345 was conducted on 2023-10-15. Status: Action Required. There is 1 issue and 1 pending fix.

---

**👤 You:**
> "Are there any pending safety fixes I need to address?"

**🤖 AI Agent:**
> Yes, there is 1 pending action item: Fix the stuck back door (from drill 12345).


## ❓ FAQ

**Q: How do I record a new drill?**
You can use the `record_drill_session` tool to input the drill date, participants, route, meeting point, and any issues found.

**Q: How can I see what needs to be fixed?**
Use the `list_action_items` tool to retrieve a list of all unresolved issues and assigned fixes that require attention.

**Q: What makes a drill 'follow-up-ready'?**
A drill is follow-up-ready when the `reviewDate` has passed and all `assignedFixes` have been addressed, which you can verify with `verify_drill_readiness`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/household-safety-drill-record](https://vinkius.com/en/ai-agent-connect/household-safety-drill-record)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Household Safety Drill Record** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `household-safety-drill-record` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Household Safety Drill Record** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "household-safety-drill-record": {
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
