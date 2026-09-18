# Peaking Index Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/peaking-index-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Model athletic readiness using the Banister Fitness-Fatigue model.

## Description
This MCP server connects AI agents to the Banister Fitness-Fatigue model, allowing for precise athletic readiness modeling. By analyzing training load and decay rates, agents can use `calculate_peaking_index` to project performance for specific competition dates. The server also provides tools like `assess_readiness` to interpret physiological states and `predict_peak_day` to identify the optimal window for peak performance. It is designed to help coaches and athletes quantify the balance between long-term fitness and short-term fatigue.


## Available Tools (5)
- **get_fatigue_level**: Quantifies the immediate physiological strain accumulated from recent training
- **get_fitness_level**: Determines the current physiological capacity of the athlete based on historical training
- **assess_readiness**: Provides a qualitative status of the athlete's readiness for competition
- **calculate_peaking_index**: Calculates the net readiness value for a specific competition date
- **predict_peak_day**: Identifies the optimal date for competition to maximize the peaking index


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Peaking Index Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Based on my training history, when is my best day to compete?"

**🤖 AI Agent:**
> Your optimal competition day is in 12 days, where your predicted peaking index will reach its maximum value.

---

**👤 You:**
> "Calculate my peaking index for a race in 7 days."

**🤖 AI Agent:**
> Your projected peaking index for the race in 7 days is 42.5, with a fitness level of 85.0 and a fatigue level of 42.5.

---

**👤 You:**
> "Am I ready for my marathon next week?"

**🤖 AI Agent:**
> Your current status is 'Peaked', meaning you are in an optimal state for competition with high fitness and manageable fatigue.


## ❓ FAQ

**Q: How does the peaking index work?**
The index is calculated by projecting fitness and fatigue levels forward to a target date. It represents the net difference between the two, where a higher value indicates better readiness.

**Q: Can I find the best day for my race?**
Yes, you can use the `predict_peak_day` tool to scan a future window of days and identify when your peaking index is projected to be at its maximum.

**Q: What is a 'Detrained' status?**
A 'Detrained' status occurs when both fitness and fatigue levels are low, indicating a lack of recent training stimulus.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/peaking-index-calculator](https://vinkius.com/en/ai-agent-connect/peaking-index-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Peaking Index Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `peaking-index-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Peaking Index Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "peaking-index-calculator": {
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
