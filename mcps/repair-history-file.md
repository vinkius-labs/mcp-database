# Repair History File MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/repair-history-file)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automotive](../categories/automotive.md)

Transform fragmented service data into structured, chronological maintenance records.

## Description
This MCP server connects AI agents to service data, allowing technicians to retrieve organized maintenance timelines. Use `get_chronological_history` to view a full timeline of service events, `analyze_symptom_patterns` to identify recurring issues, `filter_warranty_records` to audit warranty claims, and `summarize_part_usage` to track component replacement frequency.


## Available Tools (4)
- **analyze_symptom_patterns**: Identify repeating symptoms across the history to understand if a current issue is recurring
- **filter_warranty_records**: Isolate service events that were processed as warranty claims or non-warranty repairs
- **get_chronological_history**: Provide a single, ordered timeline of all recorded service events for a specific asset
- **summarize_part_usage**: Provide a high-level view of which components are most frequently replaced for a specific asset


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Repair History File** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the maintenance history for asset ID 12345."

**🤖 AI Agent:**
> Here is the chronological history for asset 12345: 2023-01-15: Oil change; 2023-06-10: Brake pad replacement; 2024-02-01: Battery replacement.

---

**👤 You:**
> "Has this vehicle had engine overheating issues before?"

**🤖 AI Agent:**
> Yes, engine overheating was recorded on 2023-05-12 and 2023-11-20.

---

**👤 You:**
> "Which parts are replaced most often for asset 98765?"

**🤖 AI Agent:**
> The most frequently replaced parts for asset 98765 are: Brake Pads (4), Air Filters (3), and Spark Plugs (2).


## ❓ FAQ

**Q: How can I see the full history of a vehicle?**
You can use the `get_chronological_history` tool by providing the specific asset ID.

**Q: Can I check if a part replacement was covered by warranty?**
Yes, the `filter_warranty_records` tool allows you to isolate service events based on their warranty status.

**Q: How do I identify if a symptom is a recurring problem?**
Use the `analyze_symptom_patterns` tool to find previous instances of a specific symptom for an asset.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/repair-history-file](https://vinkius.com/en/ai-agent-connect/repair-history-file)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Repair History File** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `repair-history-file` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Repair History File** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "repair-history-file": {
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
