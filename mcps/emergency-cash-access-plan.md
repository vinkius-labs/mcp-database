# Emergency Cash Access Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/emergency-cash-access-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate structured contingency readiness documents for household emergency funding and contact hierarchies.

## Description
This MCP server provides tools to build comprehensive emergency readiness plans. It helps households calculate funding strategies using `get_funding_access_plan`, identify authorized responders via `get_responsible_contacts`, maintain schedules with `get_review_schedule`, and verify preparedness through `get_documentation_checklist`. It bridges the gap between household budget constraints and actionable emergency protocols.


## Available Tools (4)
- **get_responsible_contacts**: Identifies who is authorized to act and how they should be reached
- **get_documentation_checklist**: Produces a list of items that must be prepared or verified for the plan to be valid
- **get_funding_access_plan**: Calculates the specific financial readiness strategy based on budget and caps
- **get_review_schedule**: Generates a maintenance calendar to keep the plan updated


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Emergency Cash Access Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a funding strategy for a $5000 budget with a $500 spending cap using a home safe."

**🤖 AI Agent:**
> Your strategy is a Tier 2 approach with $5000 available liquidity and a $500 single-event limit, stored in a home safe.

---

**👤 You:**
> "Who is my primary responder if I have John Doe and Jane Doe as authorized adults?"

**🤖 AI Agent:**
> John Doe is your primary responder.

---

**👤 You:**
> "When is my next plan review if my last one was on 2024-01-01 and I review quarterly?"

**🤖 AI Agent:**
> Your next review date is 2024-04-01.


## ❓ FAQ

**Q: How do I calculate my emergency funding strategy?**
You can use the `get_funding_access_plan` tool by providing your total liquid budget, spending caps, and preferred storage method.

**Q: Can I manage my emergency contact list?**
Yes, the `get_responsible_contacts` tool identifies authorized adults and maps their specific access permissions.

**Q: How often should I update my plan?**
You can use `get_review_schedule` to automatically calculate your next review date based on your chosen frequency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/emergency-cash-access-plan](https://vinkius.com/en/ai-agent-connect/emergency-cash-access-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Emergency Cash Access Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `emergency-cash-access-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Emergency Cash Access Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "emergency-cash-access-plan": {
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
