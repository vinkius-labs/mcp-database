# Co-Parenting Logistics Brief MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/co-parenting-logistics-brief)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A logistics coordination engine for managing parenting agreements, schedules, and neutral communications.

## Description
This MCP server acts as a bridge between parenting agreements and AI agents. It processes complex custodial schedules, responsibility assignments, and expense tracking to minimize conflict. Using tools like `generate_exchange_calendar` and `list_responsibilities`, agents can provide parents with precise transition dates and duty lists. The `record_expense_handoff` tool ensures financial tracking follows the agreed rules, while `compose_neutral_message` generates factual, non-emotional communication templates to facilitate smooth coordination.


## Available Tools (4)
- **compose_neutral_message**: To generate a factual, non-emotional text template for communicating schedule changes or confirmations
- **generate_exchange_calendar**: To provide a structured view of upcoming custody transitions based on the current agreement
- **list_responsibilities**: To identify which parent is responsible for specific tasks during a given timeframe
- **record_expense_handoff**: To log a new expense and prepare it for reconciliation against the agreement


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Co-Parenting Logistics Brief** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the upcoming exchange schedule for next week."

**🤖 AI Agent:**
> The upcoming exchanges for next week are: Monday, Oct 2nd at 5:00 PM at the Central Library (Parent A to Parent B) and Thursday, Oct 5th at 8:00 AM at the School (Parent B to Parent A).

---

**👤 You:**
> "What are my responsibilities for tomorrow?"

**🤖 AI Agent:**
> On October 1st, your responsibilities include: School drop-off at 8:00 AM at West Elementary and Medical appointment at 3:00 PM at City Clinic.

---

**👤 You:**
> "I need to tell the other parent that the pickup location for Friday has changed to the park."

**🤖 AI Agent:**
> Subject: Schedule Change - Friday Pickup. The pickup location for Friday, October 6th, has been changed to Central Park at 5:00 PM.


## ❓ FAQ

**Q: How does this tool ensure communication remains neutral?**
The `compose_neutral_message` tool uses the provided agreement rules to strip emotional subtext, focusing only on factual data like dates, times, and locations.

**Q: Can I use this to track school-related expenses?**
Yes, by using `record_expense_handoff`, you can log educational costs and the system will determine the responsible party based on your agreement.

**Q: How do I see upcoming custody handoffs?**
You can use the `generate_exchange_calendar` tool to view a structured list of upcoming transitions, including locations and transport responsibilities.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/co-parenting-logistics-brief](https://vinkius.com/en/ai-agent-connect/co-parenting-logistics-brief)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Co-Parenting Logistics Brief** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `co-parenting-logistics-brief` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Co-Parenting Logistics Brief** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "co-parenting-logistics-brief": {
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
