# Running Pace Equivalent MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/running-pace-equivalent)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Predict equivalent race times and training zones using physiological performance models.

## Description
This MCP server connects AI agents to physiological running models to calculate race performance metrics. By providing a known race distance and time, you can use `predict_equivalent_time` to estimate your performance at different distances. You can also use `get_training_zones` to derive specific training paces like easy, threshold, and interval intensities based on your current fitness. Additionally, `compare_performances` helps determine the difference between your current training pace and a target race pace.


## Available Tools (4)
- **compare_performances**: Compares a target race pace against a current training pace
- **get_distance_constants**: Returns the list of standard racing distances recognized by the system
- **get_training_zones**: Calculates training intensity zones based on a known race performance
- **predict_equivalent_time**: Predicts equivalent race time for a target distance based on a known performance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Running Pace Equivalent** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "If I ran a 5k in 25 minutes, what would my marathon time be?"

**🤖 AI Agent:**
> Based on your 5k time, your predicted marathon time is 3:45:12 with a pace of 5:20 min/km.

---

**👤 You:**
> "What should my training paces be if I recently ran a 10k in 50 minutes?"

**🤖 AI Agent:**
> Your training zones are: Easy pace 6:15 min/km, Threshold pace 5:10 min/km, and Interval pace 4:35 min/km.

---

**👤 You:**
> "My current training pace is 5:30 min/km. How does this compare to a target race pace of 5:00 min/km?"

**🤖 AI Agent:**
> The target race pace is 30 seconds per km faster than your current training pace.


## ❓ FAQ

**Q: How do I know which distances are supported?**
You can use the `get_distance_constants` tool to retrieve the full list of standard racing distances recognized by the system.

**Q: What is a VDOT score?**
A VDOT score is a single numerical value representing your aerobic capacity, used to predict race times and training intensities.

**Q: Can I compare my training pace to a race pace?**
Yes, the `compare_performances` tool allows you to compare your current training pace against a target race pace.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/running-pace-equivalent](https://vinkius.com/en/ai-agent-connect/running-pace-equivalent)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Running Pace Equivalent** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `running-pace-equivalent` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Running Pace Equivalent** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "running-pace-equivalent": {
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
