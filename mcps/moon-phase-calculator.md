# Moon Phase Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/moon-phase-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate precise lunar phases, illumination, and moon age for any date.

## Description
This MCP server provides deterministic lunar phase calculations. Use `get_lunar_phase` to retrieve the moon's age, current phase name, illumination percentage, and the number of days until the next Full or New Moon for any specific date. You can also use `get_phase_sequence` to see the order of lunar phases or `get_illumination_thresholds` to understand how phases are categorized.


## Available Tools (3)
- **get_illumination_thresholds**: Identifies the logical boundaries used to categorize a moon's phase based on its illumination
- **get_lunar_phase**: Calculates the current lunar state for a specific date
- **get_phase_sequence**: Provides the ordered list of possible moon phase names


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moon Phase Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was the moon phase on 2024-07-21?"

**🤖 AI Agent:**
> On July 21, 2024, the moon was in the Full Moon phase with 100% illumination.

---

**👤 You:**
> "How much illumination will the moon have on 2024-01-01?"

**🤖 AI Agent:**
> On January 1, 2024, the moon had an illumination of approximately 45%.

---

**👤 You:**
> "When is the next Full Moon after 2024-05-10?"

**🤖 AI Agent:**
> The next Full Moon after May 10, 2024, will occur in 4 days.


## ❓ FAQ

**Q: How accurate are the lunar phase calculations?**
The calculations use a deterministic trigonometric approximation of the 29.53-day synodic month to provide highly reliable lunar data.

**Q: Can I check the moon phase for a date in the past or future?**
Yes, by using the `get_lunar_phase` tool, you can provide any date in YYYY-MM-DD format to calculate the lunar state for that specific time.

**Q: What information is returned for a specific date?**
You will receive the moon's age in days, the current phase name, the illumination percentage, and the days remaining until the next Full and New Moon.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/moon-phase-calculator](https://vinkius.com/ai-agent-connect/moon-phase-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moon Phase Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moon-phase-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moon Phase Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moon-phase-calculator": {
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
