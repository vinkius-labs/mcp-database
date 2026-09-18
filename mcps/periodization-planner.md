# Periodization Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/periodization-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Systematic training schedule generator using periodization principles.

## Description
Periodization Planner connects AI agents to professional athletic programming. It uses scientific principles to divide training into mesocycles, managing the inverse relationship between volume and intensity. Use `get_mesocycle_structure` to define training blocks, `calculate_weekly_progression` to set specific weekly targets, `get_recovery_strategy` to identify necessary deload weeks, and `summarize_training_plan` for a high-level overview of the entire strategy.


## Available Tools (4)
- **calculate_weekly_progression**: Provides the specific volume and intensity targets for every week within the generated mesocycles
- **get_mesocycle_structure**: Determines how the training period is divided into specific blocks leading up to the competition
- **get_recovery_strategy**: Informs the athlete when and how to perform deloads to ensure physiological adaptation
- **summarize_training_plan**: Provides a high-level overview of the entire training periodization strategy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Periodization Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a training structure for a marathon runner in the Preparatory phase using Linear periodization."

**🤖 AI Agent:**
> The training period is divided into three mesocycles: a foundational base block, a strength-building block, and a pre-competition block, following a linear progression of decreasing volume and increasing intensity.

---

**👤 You:**
> "What is the weekly volume and intensity for an advanced strength athlete?"

**🤖 AI Agent:**
> For an advanced athlete, the weekly schedule shows high-intensity peaks with precise volume management to trigger adaptation while preventing overtraining.

---

**👤 You:**
> "Summarize my training plan for a power sport."

**🤖 AI Agent:**
> The training plan spans 12 weeks, with a peak intensity occurring in week 10, focusing on explosive power development.


## ❓ FAQ

**Q: How does the planner handle different athlete levels?**
The planner adjusts volume and intensity progression based on the athlete level. For example, `calculate_weekly_progression` uses the athlete level to determine how steeply intensity climbs and how frequently recovery is needed.

**Q: Can I choose between linear and undulating models?**
Yes, you can specify the `periodizationModel` in `get_mesocycle_structure` to choose between Linear or Undulating approaches.

**Q: How are recovery weeks determined?**
Recovery weeks are strategically identified using `get_recovery_strategy`, which places deloads at the end of high-stress mesocycles to ensure physiological adaptation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/periodization-planner](https://vinkius.com/en/ai-agent-connect/periodization-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Periodization Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `periodization-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Periodization Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "periodization-planner": {
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
