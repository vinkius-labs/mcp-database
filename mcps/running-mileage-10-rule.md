# Running Mileage 10% Rule MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/running-mileage-10-rule)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [training](../categories/training.md)

Generate safe running progression plans using the 10% growth rule.

## Description
This MCP server provides a safety-first training progression generator. Use `generate_mileage_plan` to create a week-by-week schedule from your current mileage to a target goal, adhering to the 10% growth rule and a 12% volatility cap. You can also use `calculate_next_step` to find your next recommended distance or `validate_transition_safety` to audit proposed increases.


## Available Tools (3)
- **calculate_next_step**: Determines the safest mileage for the next training week
- **generate_mileage_plan**: Generates a full week-by/week training schedule
- **validate_transition_safety**: Audits a proposed mileage increase


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Running Mileage 10% Rule** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a running plan starting at 10km and reaching 15km."

**🤖 AI Agent:**
> [10, 11, 12, 13, 14, 15]

---

**👤 You:**
> "What should my mileage be next week if I ran 20km this week?"

**🤖 AI Agent:**
> Your recommended mileage for next week is 22km.

---

**👤 You:**
> "Is it safe to jump from 5km to 7km?"

**🤖 AI Agent:**
> No, a jump from 5km to 7km is a 40% increase, which exceeds the 12% safety limit.


## ❓ FAQ

**Q: How does the 10% rule work?**
It increases weekly mileage by 10% each week to allow for physiological adaptation. You can use `calculate_next_step` to see your next step.

**Q: What is the volatility cap?**
To prevent large jumps due to rounding, any increase exceeding 12% is capped. Use `validate_transition_safety` to check any jump.

**Q: Can I generate a full training plan?**
Yes, use `generate_mileage_plan` with your starting and target mileage to get a complete weekly schedule.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/running-mileage-10-rule](https://vinkius.com/mcp/running-mileage-10-rule)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Running Mileage 10% Rule** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `running-mileage-10-rule` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Running Mileage 10% Rule** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "running-mileage-10-rule": {
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
