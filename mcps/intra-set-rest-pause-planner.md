# Intra-Set Rest-Pause Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/intra-set-rest-pause-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [training](../categories/training.md)

Design high-intensity rest-pause protocols to maximize effective repetitions.

## Description
This MCP server provides specialized tools for designing high-intensity rest-pause training protocols. By analyzing current fatigue and target repetition goals, it generates precise tactical plans including cluster distributions and mini-rest timings. Use `plan_rest_pause_sequence` to create a complete set structure, `analyze_fatigue_impact` to adjust for exhaustion, `validate_repetition_distribution` to ensure mathematical accuracy, and `calculate_effective_reps_score` to estimate the hypertrophic stimulus of your training session.


## Available Tools (4)
- **analyze_fatigue_impact**: Calculates how the current fatigue level will specifically alter the rest intervals and rep density
- **calculate_effective_reps_score**: Provides a single score representing the hypertrophic stimulus of a planned sequence
- **plan_rest_pause_sequence**: Generates a complete tactical plan for a single rest-pause set based on user goals and fatigue
- **validate_repetition_distribution**: Ensures a proposed set of rep clusters is mathematically sound and follows the requested rest-pause type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Intra-Set Rest-Pause Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a rest-pause set for Bench Press with a goal of 12 total reps, current fatigue at 4, using a descending methodology."

**🤖 AI Agent:**
> Your plan for Bench Press: Perform 5 reps, rest 30 seconds, perform 4 reps, rest 30 seconds, then perform 3 reps.

---

**👤 You:**
> "How much will my current fatigue of 8 impact my rest intervals?"

**🤖 AI Agent:**
> With a fatigue level of 8, your rest adjustment factor is increased, meaning you will need longer mini-rests to maintain intensity.

---

**👤 You:**
> "Is a distribution of 5, 4, 3 valid for a 12 rep goal using descending rest?"

**🤖 AI Agent:**
> Yes, the distribution 5-4-3 is valid for a descending methodology as each subsequent cluster is smaller than the previous one.


## ❓ FAQ

**Q: What is a rest-pause protocol?**
It is a high-intensity technique where a set is broken into small clusters of repetitions separated by very short rest periods to increase effective repetitions.

**Q: How does fatigue affect my plan?**
Higher fatigue levels will result in smaller repetition clusters and longer mini-rest intervals to ensure you can still hit your target stimulus.

**Q: Can I use this with Claude or Cursor?**
Yes, you can connect this via Vinkius Edge to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/intra-set-rest-pause-planner](https://vinkius.com/en/ai-agent-connect/intra-set-rest-pause-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Intra-Set Rest-Pause Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `intra-set-rest-pause-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Intra-Set Rest-Pause Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "intra-set-rest-pause-planner": {
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
