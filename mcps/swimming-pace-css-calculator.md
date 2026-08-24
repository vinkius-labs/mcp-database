# Swimming Pace & CSS Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/swimming-pace-css-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate precise swimming splits, pacing, and Critical Swim Speed (CSS).

## Description
A deterministic utility for swimmers to plan training sessions. Use `calculate_pace_and_splits` to determine required pace per 100 units, exact split times for every pool length, and total turn counts. Use `calculate_css` to estimate your aerobic threshold based on test times. The tool accounts for stroke-specific drag coefficients for freestyle, backstroke, breaststroke, and butterfly to ensure accurate pacing.


## Available Tools (3)
- **calculate_css**: 
- **calculate_pace_and_splits**: 
- **validate_swimming_parameters**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Swimming Pace & CSS Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the splits for a 400m freestyle swim in a 25m pool with a target time of 05:00."

**🤖 AI Agent:**
> For a 400m freestyle in a 25m pool with a 05:00 target, your pace per 100m is 01:15. You will perform 15 turns, and your splits are: 00:15, 00:30, 00:45, 01:00, 01:15, 01:30, 01:45, 02:00, 02:15, 02:30, 02:45, 03:00, 03:15, 03:30, 03:45, 04:00, 04:15, 04:30, 04:45, 05:00.

---

**👤 You:**
> "What is my CSS if my 3000m time was 45:00 and my 400m time was 06:00?"

**🤖 AI Agent:**
> Your calculated Critical Swim Speed (CSS) pace is 01:30 per 100m.

---

**👤 You:**
> "Can I swim 100m in a 50m pool?"

**🤖 AI Agent:**
> Yes, 100m is a multiple of 50m, so the distance and pool length are compatible.


## ❓ FAQ

**Q: How do I calculate my splits for a specific distance?**
You can use the `calculate_pace_and_splits` tool by providing the total distance, your target time, the stroke type, and the pool length.

**Q: What is Critical Swim Speed (CSS)?**
CSS is an estimate of your aerobic threshold. You can calculate it using `calculate_css` by inputting your 3000m and 400m test times.

**Q: Does the tool account for different swimming strokes?**
Yes, the tool applies specific drag coefficients for freestyle, backstroke, breaststroke, and butterfly to adjust pacing requirements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/swimming-pace-css-calculator](https://vinkius.com/ai-agent-connect/swimming-pace-css-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Swimming Pace & CSS Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `swimming-pace-css-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Swimming Pace & CSS Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "swimming-pace-css-calculator": {
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
