# Mental Performance Visualization MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/mental-performance-visualization)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [performance](../categories/performance.md)

Tailored mental rehearsal protocols for surfers to optimize performance.

## Description
This MCP server provides specialized sport psychology tools for surfers. It generates detailed visualization scripts, structured practice schedules, and calculates optimal rehearsal frequencies based on competition goals, anxiety levels, and experience. Use `get_visualization_script` to create immersive mental rehearsals, `get_practice_schedule` to plan your training, and `analyze_performance_readiness` to assess your mental state before a heat.


## Available Tools (4)
- **analyze_performance_readiness**: Evaluates how prepared the surfer is based on their training parameters and psychological state
- **calculate_rehearsal_frequency**: Determines how many times per day or per week the athlete should perform the visualization
- **get_practice_schedule**: Provides a structured calendar for performing visualization sessions leading up to a target date
- **get_visualization_script**: Generates a detailed mental rehearsal script tailored to specific surf goals and environmental conditions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mental Performance Visualization** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a visualization script for a heavy barrel scenario with high anxiety."

**🤖 AI Agent:**
> Close your eyes and breathe deeply. You are sitting on your board, watching the heavy barrel form. The sound of the water is deafening, but you are calm. As the wave peaks, you feel the sudden surge of energy...

---

**👤 You:**
> "Create a 7-day practice schedule for a novice surfer with a competition in one week."

**🤖 AI Agent:**
> Day 1: 10m session. Day 2: 15m session. Day 3: Rest. Day 4: 15m session. Day 5: 20m session. Day 6: 10m light session. Day 7: Competition Day.

---

**👤 You:**
> "How many times should I practice visualization if I am an expert with a complex goal?"

**🤖 AI Agent:**
> For an expert with a complex goal, it is recommended to perform 2 sessions per day to maintain high neural priming.


## ❓ FAQ

**Q: How can I use this to prepare for a competition?**
You can use `get_practice_schedule` to build a training plan and `get_visualization_script` to perform the actual mental rehearsals required for your specific wave scenarios.

**Q: Can I adjust the training based on my stress levels?**
Yes, the tools use your `anxietyLevel` to adjust the tone of the scripts and the frequency of the sessions to ensure optimal mental state.

**Q: How do I know if I am ready for my heat?**
Use the `analyze_performance_readiness` tool to compare your completed sessions against your planned schedule and receive a readiness score.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/mental-performance-visualization](https://vinkius.com/en/ai-agent-connect/mental-performance-visualization)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mental Performance Visualization** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mental-performance-visualization` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mental Performance Visualization** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mental-performance-visualization": {
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
