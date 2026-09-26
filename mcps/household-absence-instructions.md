# Household Absence Instructions MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/household-absence-instructions)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate structured, day-by-day caretaker guides from travel schedules and care requirements.

## Description
This MCP server transforms disparate travel dates, property maintenance needs, and biological care instructions into a cohesive, chronological caretaker manual. It uses `generate_daily_guide` to expand recurring tasks into a specific timeline, `validate_care_schedule` to detect logical conflicts, `summarize_access_protocol` for quick entry reference, and `map_escalation_path` to organize emergency contacts by severity.


## Available Tools (4)
- **map_escalation_path**: 
- **summarize_access_protocol**: 
- **validate_care_schedule**: 
- **generate_daily_guide**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Household Absence Instructions** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a daily guide for my trip from 2024-06-01 to 2024-06-05. I need to water plants every 2 days at 10:00 AM and feed my cat daily at 8:00 AM."

**🤖 AI Agent:**
> Guide Title: Trip Care Schedule

2024-06-01
- 08:00 AM: Feed cat
- 10:00 AM: Water plants

2024-06-02
- 08:00 AM: Feed cat

2024-06-03
- 08:00 AM: Feed cat
- 10:00 AM: Water plants

2024-06-04
- 08:00 AM: Feed cat

2024-06-05
- 08:00 AM: Feed cat
- 10:00 AM: Water plants

---

**👤 You:**
> "Summarize my entry instructions: Keypad code is 1234 and there is a physical key under the mat."

**🤖 AI Agent:**
> Primary Method: Keypad
All Methods:
- Keypad: 1234
- Physical Key: under the mat

---

**👤 You:**
> "What is the contact hierarchy? Primary is John (Routine), Secondary is Jane (Urgent), and Emergency is 911."

**🤖 AI Agent:**
> 1. Emergency: 911
2. Urgent: Jane
3. Routine: John


## ❓ FAQ

**Q: How do I create a daily schedule?**
Provide your travel dates and care requirements to the `generate_daily_guide` tool to receive a complete day-by-day manual.

**Q: Can the tool check for scheduling conflicts?**
Yes, use the `validate_care_schedule` tool to identify impossible care requirements or overlapping tasks.

**Q: How are emergency contacts handled?**
The `map_escalation_path` tool organizes your contacts into a hierarchy based on the severity of the situation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/household-absence-instructions](https://vinkius.com/en/ai-agent-connect/household-absence-instructions)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Household Absence Instructions** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `household-absence-instructions` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Household Absence Instructions** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "household-absence-instructions": {
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
