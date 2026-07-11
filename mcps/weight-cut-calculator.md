# Weight Cut Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/weight-cut-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health-fitness](../categories/health-fitness.md)

Calculate safe water cut limits, daily weight loss pace, and hydration protocols for combat sports.

## Description
The `weight_cut_calculator` tool provides a specialized planning utility for combat sports athletes. It calculates the safe water cut limit based on your weigh-in type, determines the necessary daily weight loss pace, and outlines detailed timelines for water loading, sodium manipulation, and post-weigh-in rehydration strategies. Use it to manage body mass changes through fluid and electrolyte regulation while staying within physiological safety thresholds.


## Available Tools (1)
- **weight_cut_calculator**: Calculate required weight loss parameters for an athlete


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Weight Cut Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I weigh 180 lbs and need to hit 170 lbs for a same-day weigh-in in 5 days. Is this safe?"

**🤖 AI Agent:**
> A cut from 180 to 170 lbs is approximately 5.5%. Since this is below the 8% threshold for same-day weigh-ins, it is considered within the optimal safety zone.

---

**👤 You:**
> "Calculate my weight loss pace if I am at 75kg and need to reach 70kg by next week."

**🤖 AI Agent:**
> To reach 70kg from 75kg in 7 days, you need to lose a total of 5kg at an average daily pace of approximately 0.71kg per day.

---

**👤 You:**
> "What is the plan for sodium manipulation?"

**🤖 AI Agent:**
> The protocol includes a loading phase with high sodium intake to facilitate osmotic loading, followed by a depletion phase where sodium is minimized to trigger fluid excretion.


## ❓ FAQ

**Q: How safe is my weight cut?**
The tool evaluates safety based on your weigh-in type. For same-day weigh-ins, it flags any cut exceeding 8% as a RED WARNING. For next-day weigh-ins, the limit is 10%.

**Q: What does the water loading protocol include?**
It provides a detailed timeline for increasing water intake to stimulate flushing, followed by a progressive taper and restriction phase leading up to your weigh-in.

**Q: Can I use this for MMA or Wrestling?**
Yes, it is specifically designed for any combat sport athlete (MMA, Wrestling, BJJ, Boxing) needing to manage weight through fluid and electrolyte manipulation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/weight-cut-calculator](https://vinkius.com/mcp/weight-cut-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Weight Cut Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `weight-cut-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Weight Cut Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "weight-cut-calculator": {
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
