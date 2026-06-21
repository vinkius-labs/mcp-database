# Training Load Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/training-load-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Quantify training stress, detect overtraining risks, and generate recovery strategies.

## Description
This MCP server provides specialized tools to manage physical training load. Use `calculate_session_load` to determine the total physiological stress of a single session by multiplying volume and perceived intensity. Monitor your progress with `analyze_overtraining_risk`, which compares your current weekly load against a baseline to identify potential fatigue or overreaching. If recovery is needed, use `generate_deload_strategy` to receive specific targets for volume and intensity reduction, helping you maintain fitness while dissipating accumulated fatigue.


## Available Tools (3)
- **generate_deload_strategy**: Generates specific training targets for an upcoming recovery (deload) week
- **analyze_overtraining_risk**: Evaluates whether current training patterns indicate a high risk of overtraining
- **calculate_session_load**: Calculates the total physical stress for a single completed training session


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Training Load Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the load for a session with 5000kg volume and an RPE of 8."

**🤖 AI Agent:**
> The `calculate_session_load` tool would return a session load of 40000.

---

**👤 You:**
> "Check my overtraining risk with a weekly load of 50000 and a baseline of 40000."

**🤖 AI Agent:**
> The `analyze_overtraining_risk` tool would evaluate the increase in load and provide your current risk status and level.

---

**👤 You:**
> "Generate a deload strategy for 3000kg volume and intensity 7, reducing by 25%."

**🤖 AI Agent:**
> The `generate_deload_strategy` tool will calculate the new target volume of 2250kg and a reduced intensity level.


## ❓ FAQ

**Q: How is training load calculated?**
The session load is calculated by multiplying the total volume of work (e.g., kilograms or kilometers) by the Rate of Perceived Exertion (RPE).

**Q: What does overtraining risk analysis involve?**
The tool compares your current weekly training load against a stable baseline load to determine if you are in maintenance, accumulation, or at risk of overtraining.

**Q: How can I use the deload strategy tool?**
Provide your most recent training volume and intensity, and optionally a reduction percentage. The tool will then generate specific targets for your recovery week.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/training-load-calculator](https://vinkius.com/mcp/training-load-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Training Load Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `training-load-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Training Load Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "training-load-calculator": {
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
