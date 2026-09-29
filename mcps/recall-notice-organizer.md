# Recall Notice Organizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/recall-notice-organizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Organizes vehicle recall notices into prioritized appointment plans.

## Description
This MCP server acts as an intelligent triage system for vehicle owners. It processes raw recall notices and organizes them into actionable appointment plans by evaluating urgency, remedy availability at local dealers, and user time constraints. Using tools like `analyze_recall_notices` and `filter_ready_dealers`, it identifies which repairs can be scheduled immediately and which remain unresolved due to part shortages or dealer capacity. It helps users prioritize safety-critical repairs over maintenance tasks.


## Available Tools (4)
- **analyze_recall_notices**: 
- **calculate_appointment_window**: 
- **filter_ready_dealers**: 
- **get_urgency_weight**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Recall Notice Organizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Organize these recall notices: [{"noticeId": "R1", "description": "Brake failure", "urgencyLevel": "Critical", "date": "2023-10-01"}] with dealer status [{"dealerName": "Main St Motors", "partsAvailable": ["R1"], "openSlots": ["2023-10-05"]}] and user availability {"maxTime": 120}."

**🤖 AI Agent:**
> {"prioritizedAppointments": [{"noticeId": "R1", "dealerName": "Main St Motors", "estimatedDuration": 60, "urgency": "Critical"}], "unresolvedNotices": []}

---

**👤 You:**
> "Check if a 90-minute repair fits in my 60-minute window."

**🤖 AI Agent:**
> {"isFeasible": false}

---

**👤 You:**
> "Which dealers have parts for recall R1?"

**🤖 AI Agent:**
> {"availableDealers": [{"dealerName": "Main St Motors", "nextAvailableSlot": "2023-10-05"}]}


## ❓ FAQ

**Q: How does the system decide which recall to fix first?**
The system uses `get_urgency_weight` to prioritize recalls based on safety risk, ensuring critical safety issues are addressed before maintenance tasks.

**Q: Why is a recall listed as unresolved?**
A recall is marked as unresolved if the required parts are not in stock at nearby dealers or if no appointment slots are available within your specified time window.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/recall-notice-organizer](https://vinkius.com/en/ai-agent-connect/recall-notice-organizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Recall Notice Organizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `recall-notice-organizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Recall Notice Organizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "recall-notice-organizer": {
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
