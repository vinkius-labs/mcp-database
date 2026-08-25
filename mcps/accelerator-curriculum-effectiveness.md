# Accelerator Curriculum Effectiveness MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-curriculum-effectiveness)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Measure the impact and quality of accelerator training programs through multi-dimensional performance metrics.

## Description
This MCP server provides a specialized measurement system to evaluate the impact and quality of accelerator training programs. By analyzing the interplay between participation, satisfaction, and learning outcomes, it provides a holistic view of curriculum health. Use `get_engagement_metrics` to track participant participation, `get_learning_impact` to measure educational value, and `analyze_curriculum_health` to receive actionable recommendations for program improvement.


## Available Tools (3)
- **curriculum_health**: Provide actionable insights and recommended changes based on a full set of program data
- **engagement_metrics**: Determine how well participants are showing up and participating in scheduled sessions
- **learning_impact**: Measure the educational value and effectiveness of the curriculum in achieving goals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Curriculum Effectiveness** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How engaged were my participants if I delivered 10 sessions with an 85% attendance rate in a synchronous format?"

**🤖 AI Agent:**
> Your engagement score is 88.5, reflecting high participation in your synchronous sessions.

---

**👤 You:**
> "What is the learning impact for a program with a 75% completion rate and a 0.8 outcome correlation?"

**🤖 AI Agent:**
> The learning impact score is 60, and the completion status is medium.

---

**👤 You:**
> "Analyze the health of my curriculum: 12 sessions, 80% attendance, 70% completion, 8 satisfaction, 0.7 correlation, and morning sessions."

**🤖 AI Agent:**
> Your overall health score is 76. Recommended changes: Increase engagement by adjusting session timing.


## ❓ FAQ

**Q: How does the system calculate engagement?**
Engagement is calculated by analyzing the relationship between sessions delivered and the attendance rate, with adjustments made based on the delivery format via `get_engagement_metrics`.

**Q: Can I get recommendations for improving my curriculum?**
Yes, by using the `analyze_curriculum_health` tool, the system provides specific, natural language suggestions to improve engagement, impact, or satisfaction.

**Q: What metrics are used for learning impact?**
Learning impact is determined by combining the completion rate with the outcome correlation using the `get_learning_impact` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-curriculum-effectiveness](https://vinkius.com/ai-agent-connect/accelerator-curriculum-effectiveness)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Curriculum Effectiveness** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-curriculum-effectiveness` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Curriculum Effectiveness** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-curriculum-effectiveness": {
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
