# Sports Training Load Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sports-training-load-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Quantify training load, monitor injury risk, and analyze training patterns.

## Description
This MCP server provides a specialized engine for quantifying physical exertion and monitoring athletic readiness. It allows AI agents to calculate specific session loads using `analyze_session_load`, determine injury risk via the Acute:Chronic Workload Ratio with `calculate_fitness_readiness`, and identify overtraining risks through `evaluate_training_pattern`. Coaches and athletes can also use `summarize_weekly_metrics` to get high-level overviews of volume and intensity.


## Available Tools (4)
- **analyze_session_load**: Calculates the specific load for a single training session
- **calculate_fitness_readiness**: Determines the athlete's current readiness and injury risk
- **evaluate_training_pattern**: Analyzes the variety of training to identify risks of overtraining
- **summarize_weekly_metrics**: Provides a high-level overview of training volume and intensity for a specific week


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sports Training Load Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the load for a 45-minute aerobic run with an RPE of 7."

**🤖 AI Agent:**
> The calculated training load for your 45-minute aerobic session is 315.

---

**👤 You:**
> "What is my current fitness readiness based on this history: [{"load": 100, "date": "2023-10-01"}, {"load": 120, "date": "2023-10-02"}]?"

**🤖 AI Agent:**
> Based on the provided history, your current status is Underloaded.

---

**👤 You:**
> "Summarize my training for the week starting 2023-10-01 with this history: [{"load": 50, "distance": 5, "date": "2023-10-01"}, {"load": 60, "distance": 6, "date": "2023-10-02"}]"

**🤖 AI Agent:**
> For the week starting 2023-10-01, your total load was 110, with an average daily load of 55 and a total distance of 11 km across 2 sessions.


## ❓ FAQ

**Q: How do I calculate the load for a single session?**
You can use the `analyze_session_load` tool by providing the session duration, RPE, and the type of exercise performed.

**Q: Can this tool help prevent injuries?**
Yes, by using `calculate_fitness_readiness`, the tool monitors the Acute:Chronic Workload Ratio to identify sudden spikes in training that increase injury risk.

**Q: How is monotony measured?**
The `evaluate_training_pattern` tool calculates monotony by analyzing the variance in your daily training loads.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sports-training-load-calculator](https://vinkius.com/en/ai-agent-connect/sports-training-load-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sports Training Load Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sports-training-load-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sports Training Load Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sports-training-load-calculator": {
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
