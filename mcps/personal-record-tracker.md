# Personal Record Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/personal-record-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Predictive analytics for athletes to track PRs and forecast performance peaks.

## Description
This MCP server provides predictive analytics for athletes to track historical personal records (PRs) and forecast future performance peaks. By analyzing historical data and current training states, it calculates progression rates and target values. Use `get_progression_metrics` to understand improvement velocity, `project_next_targets` to set realistic goals for upcoming cycles, and `calculate_achievement_probability` to assess the likelihood of hitting specific targets. It also provides phase-specific insights via `get_training_phase_impact` to adjust expectations based on current training intensity.


## Available Tools (4)
- **calculate_achievement_probability**: Estimate the probability of hitting a specific target value
- **get_progression_metrics**: Each entry must be a JSON string representing an object with "value" (number) and "date" (ISO string).

Calculate athlete progression metrics from historical personal records
- **get_training_phase_impact**: Retrieve the performance multiplier and volatility for a training phase
- **project_next_targets**: Project future personal record targets based on training phase and timeline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Personal Record Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How fast am I improving based on my last 5 PRs?"

**🤖 AI Agent:**
> Your average progression rate is 2.5kg per month with a stable trend direction.

---

**👤 You:**
> "What is my target squat for 30 days from now if I am in the Intensification phase?"

**🤖 AI Agent:**
> Your projected target squat for 30 days from now is 145kg, with a confidence interval of +/- 2kg.

---

**👤 You:**
> "What is the probability I will hit a 200kg deadlift in the next 60 days?"

**🤖 AI Agent:**
> There is a 65% probability of hitting 200kg within the next 60 days given your current trajectory.


## ❓ FAQ

**Q: How accurate are the performance projections?**
Projections are based on your historical progression rate and current training phase. While they provide statistical estimates, actual performance depends on physiological factors and training adherence.

**Q: What data do I need to provide for a projection?**
To use `project_next_targets`, you should provide your historical PR history, recent performance data, your current training phase, and the number of days into the future you wish to project.

**Q: Can I use this to plan my peaking phase?**
Yes. You can use `get_training_phase_impact` to see how your current phase affects expected performance and use the projection tools to plan your targets for the realization phase.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/personal-record-tracker](https://vinkius.com/en/ai-agent-connect/personal-record-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Personal Record Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `personal-record-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Personal Record Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "personal-record-tracker": {
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
