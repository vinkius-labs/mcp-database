# Family Calendar Conflict Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-calendar-conflict-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Identifies scheduling overlaps and proposes deterministic alternatives based on priority and travel time.

## Description
This MCP server provides a deterministic scheduling engine to manage family commitments. It identifies temporal overlaps and impossible travel requirements using `get_conflicts`. Users can calculate free time for specific participants with `analyze_availability`, find valid rescheduling options via `propose_alternatives`, and assess the stability of schedule changes with `evaluate_priority_impact`.


## Available Tools (4)
- **analyze_availability**: Calculates the free time available for specific participants, accounting for existing commitments and necessary travel
- **evaluate_priority_impact**: Assesses how moving a specific commitment affects the overall schedule stability and priority balance
- **get_conflicts**: Identifies all overlapping commitments or impossible travel requirements for a given period
- **propose_alternatives**: Generates a set of valid, conflict-free schedules by shifting movable commitments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Calendar Conflict Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Are there any scheduling conflicts for the family between Monday and Wednesday?"

**🤖 AI Agent:**
> Yes, there is a travel impossibility conflict for Alex on Tuesday between the dentist appointment and the soccer practice.

---

**👤 You:**
> "When is Sarah free to attend a meeting on Friday afternoon?"

**🤖 AI Agent:**
> Sarah is available on Friday from 2:00 PM to 4:30 PM.

---

**👤 You:**
> "Can we move the grocery trip to a different time?"

**🤖 AI Agent:**
> Yes, the grocery trip can be moved to Thursday at 10:00 AM or Friday at 3:00 PM.


## ❓ FAQ

**Q: How does the tool handle travel time between events?**
The engine automatically accounts for required travel duration. A conflict is flagged if the end of one commitment plus the necessary travel time is later than the start of the next.

**Q: Can I move a fixed commitment?**
No. Fixed commitments have no movable window. The `propose_alternatives` tool will return an error if you attempt to move a commitment that is marked as fixed.

**Q: How is priority used in rescheduling?**
The engine respects a strict priority hierarchy. High-priority commitments cannot be moved to accommodate lower-priority ones, ensuring critical events remain stable.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-calendar-conflict-planner](https://vinkius.com/en/ai-agent-connect/family-calendar-conflict-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Calendar Conflict Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-calendar-conflict-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Calendar Conflict Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-calendar-conflict-planner": {
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
