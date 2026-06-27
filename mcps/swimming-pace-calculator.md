# Swimming Pace Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/swimming-pace-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Calculate swimming training intensities, race predictions, and efficiency metrics based on Critical Swim Speed (CSS).

## Description
An analytical tool to derive swimming training intensities, race predictions, and efficiency metrics based on Critical Swim Speed (CSS). Use `derive_css_from_base` to convert performance times into CSS pace, `calculate_training_zones` for target paces, `estimate_race_durations` for race projections, and `calculate_swolf_efficiency` for SWOLF scores.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **Swimming Pace Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I swam 400m in 6 minutes and 40 seconds. What is my CSS pace?"

**🤖 AI Agent:**
> Your CSS pace is 1:40 per 100m.

---

**👤 You:**
> "What are my training zones for a CSS of 100 seconds?"

**🤖 AI Agent:**
> Your Aerobic pace is 2:00, Threshold is 1:40, and VO2max is 1:30.

---

**👤 You:**
> "Calculate my SWOLF score for a 50s length with 20 strokes."

**🤖 AI Agent:**
> Your SWOLF score is 70.


## ❓ FAQ

**Q: What is CSS?**
Critical Swim Speed (CSS) is the estimated physiological threshold where a swimmer can maintain a steady pace without rapid fatigue. Tools available: `your_tool_name`.

**Q: How do I use `derive_css_from_base`?**
Provide your time in seconds and the distance (100m or 400m) to calculate your standardized CSS pace per 100m.

**Q: Can I predict my race times?**
Yes, use `estimate_race_durations` with your calculated CSS pace to see projected times for 200m, 400m, 800m, and 1500m.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/swimming-pace-calculator](https://vinkius.com/mcp/swimming-pace-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Swimming Pace Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `swimming-pace-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Swimming Pace Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "swimming-pace-calculator": {
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
