# Jet Lag Adjustment Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/jet-lag-adjustment-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates deterministic sleep, light, and meal schedules to mitigate jet lag.

## Description
This MCP server provides tools to manage circadian misalignment during long-haul travel. It uses principles like the Phase Response Curve to generate structured itineraries. Use `calculate_adjustment_schedule` to create a full plan, `get_phase_shift_status` to check misalignment, `validate_shift_constraints` to ensure biological safety, and `get_zeitgeber_guidance` for specific light and meal instructions.


## Available Tools (4)
- **get_zeitgeber_guidance**: Provides instructions for light and meal timing
- **calculate_adjustment_schedule**: Generates a step-by-step itinerary for adjusting to a new time zone
- **get_phase_shift_status**: Evaluates the current circadian misalignment
- **validate_shift_constraints**: Checks if a proposed sleep or light window is biologically appropriate


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jet Lag Adjustment Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a jet lag adjustment schedule for a trip from New York to Tokyo departing on July 1st at 10:00 AM and arriving on July 2nd at 2:00 PM, with a preferred sleep window of 11:00 PM to 7:00 AM and a max daily shift of 2 hours."

**🤖 AI Agent:**
> Your adjustment schedule is ready. To adjust to Tokyo time, you should advance your clock by shifting your sleep window and light exposure over the next 3 days, respecting your 2-hour daily limit.

---

**👤 You:**
> "How much am I misaligned if I am in London and the destination is Los Angeles with a 8 hour difference?"

**🤖 AI Agent:**
> You are currently experiencing an 8-hour misalignment, which is classified as a Major Shift.

---

**👤 You:**
> "What light exposure do I need to advance my clock?"

**🤖 AI Agent:**
> To advance your circadian clock, you should seek light exposure during your biological morning.


## ❓ FAQ

**Q: How do I create a full travel schedule?**
You can use the `calculate_adjustment_schedule` tool by providing your origin, destination, and preferred sleep window.

**Q: Can I check my current jet lag severity?**
Yes, the `get_phase_shift_status` tool evaluates your current misalignment and urgency.

**Q: Does this provide medical advice?**
No, this is a deterministic planning tool based on circadian biology principles, not medical advice.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/jet-lag-adjustment-planner](https://vinkius.com/en/ai-agent-connect/jet-lag-adjustment-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Jet Lag Adjustment Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jet-lag-adjustment-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Jet Lag Adjustment Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jet-lag-adjustment-planner": {
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
