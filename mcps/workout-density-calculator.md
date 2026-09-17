# Workout Density Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/workout-density-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Quantify training intensity by analyzing volume, time, and recovery.

## Description
This MCP provides precision tools to measure the efficiency of your training sessions. By analyzing the relationship between workload and time, you can calculate specific metrics like volume per minute and work-to-rest ratios. Use `get_volume_per_minute` to find your work rate, `get_work_rest_ratio` to balance recovery, `get_density_score` for a unified intensity metric, and `compare_to_benchmarks` to see how your performance stacks up against standard training tiers.


## Available Tools (4)
- **compare_to_benchmarks**: Evaluates a session's density against predefined performance tiers
- **get_density_score**: Generates a unified intensity metric for the session
- **get_work_rest_ratio**: Determines the balance between active work time and recovery time
- **get_volume_per_minute**: Calculates the rate of work performed over the total duration of the session


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Workout Density Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I lifted 5000kg over 45 minutes. What was my volume per minute?"

**🤖 AI Agent:**
> Your volume per minute was 111.11 kg/min.

---

**👤 You:**
> "My workout had 30 minutes of lifting and 15 minutes of rest. What was my work-to-rest ratio?"

**🤖 AI Agent:**
> Your work-to-rest ratio was 2.0, with 66.67% of the time spent working.

---

**👤 You:**
> "I have a density score of 45. How does this compare to standard benchmarks?"

**🤖 AI Agent:**
> A density score of 45 falls into the High tier.


## ❓ FAQ

**Q: How do I calculate my training efficiency?**
You can use the `get_density_score` tool to generate a unified intensity metric based on your total volume and duration.

**Q: Can I compare my workout to professional standards?**
Yes, the `compare_to_benchmarks` tool evaluates your density score against tiers like Moderate, High, and Elite.

**Q: What is a good work-to-rest ratio?**
Ratios vary by training goal, but you can use `get_work_rest_ratio` to determine the exact balance of your session.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/workout-density-calculator](https://vinkius.com/en/ai-agent-connect/workout-density-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Workout Density Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `workout-density-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Workout Density Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "workout-density-calculator": {
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
