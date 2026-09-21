# Contrast Therapy Timer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/contrast-therapy-timer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Plan and track timed hot and cold exposure cycles for therapeutic recovery.

## Description
This MCP server provides specialized tools to manage contrast therapy sessions. It helps users alternate between heat and cold exposure to stimulate physiological responses like vasodilation and vasoconstriction. You can use `get_session_plan` to generate a complete schedule based on your therapeutic goal, `get_next_transition` to know exactly when to switch temperatures, `validate_temperature_safety` to ensure your settings are within safe ranges, and `summary_statistics` to review the physiological load of your session.


## Available Tools (4)
- **get_next_transition**: Determines the exact time the user should switch states during an active session
- **get_session_plan**: Calculates the complete schedule of heat and cold intervals based on user parameters
- **summary_statistics**: Provides a high-level overview of the physiological load of the planned session
- **validate_temperature_safety**: Checks if the provided temperatures are biologically plausible and follow basic contrast therapy logic


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Contrast Therapy Timer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a 20-minute recovery session with 105°F hot and 55°F cold."

**🤖 AI Agent:**
> Your recovery session is set for 20 minutes. It will consist of 2 cycles, each with 5 minutes of heat at 105°F followed by 5 minutes of cold at 55°F.

---

**👤 You:**
> "I've been in the heat for 5 minutes. When should I switch to cold?"

**🤖 AI Agent:**
> You should switch to cold in 2 minutes.

---

**👤 You:**
> "What is the intensity score for a 15-minute alertness session with 110°F and 50°F?"

**🤖 AI Agent:**
> The intensity score for this session is 8.5.


## ❓ FAQ

**Q: How do I create a session schedule?**
You can use the `get_session_plan` tool by providing your desired total duration, your therapeutic goal (like recovery or alertness), and your target hot and cold temperatures.

**Q: Can I check if my temperatures are safe?**
Yes, the `validate_temperature_safety` tool checks if your chosen temperatures are biologically plausible and follow standard contrast therapy logic.

**Q: How do I know when to switch from hot to cold?**
Use the `get_next_transition` tool with your current elapsed time and your session plan to find out exactly how many minutes remain until your next temperature change.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/contrast-therapy-timer](https://vinkius.com/en/ai-agent-connect/contrast-therapy-timer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Contrast Therapy Timer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `contrast-therapy-timer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Contrast Therapy Timer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "contrast-therapy-timer": {
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
