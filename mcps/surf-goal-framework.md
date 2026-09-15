# Surf Goal Framework MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/surf-goal-framework)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transform surfing aspirations into actionable SMART goal roadmaps.

## Description
This MCP server provides a structured goal-setting framework specifically for surfers. It uses the SMART methodology to decompose high-level aspirations into a hierarchy of short-term, medium-term, and long-term goals. By distinguishing between process goals (habits) and outcome goals (results), it helps athletes build the necessary foundation for success. Use `generate_goal_roadmap` to build your plan, `get_goal_metrics` to track progress, `calculate_review_schedule` to stay on track, and `evaluate_goal_feasibility` to check if your targets are realistic.


## Available Tools (4)
- **calculate_review_schedule**: Determines when an athlete should check their progress
- **evaluate_goal_feasibility**: Analyzes if a proposed aspiration is realistic
- **generate_goal_roadmap**: Creates a structured goal framework for surfers
- **get_goal_metrics**: Retrieves specific, quantifiable measurement criteria for a defined goal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surf Goal Framework** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am an Intermediate surfer. I want to be able to ride larger waves within 6 months. Can you create a roadmap for me?"

**🤖 AI Agent:**
> Here is your 6-month surfing roadmap: Short-term goals include increasing paddle endurance and improving wave selection. Medium-term goals focus on technical maneuvers in larger swells. Long-term goals aim for consistent performance in 6-foot waves.

---

**👤 You:**
> "Is it realistic for a Beginner to win a professional contest in 3 months?"

**🤖 AI Agent:**
> No, that goal is not feasible. A Beginner requires more time to master fundamental mechanics and ocean awareness before competing at a professional level.

---

**👤 You:**
> "How often should I review my progress for my seasonal training plan?"

**🤖 AI Agent:**
> Based on a bi-weekly frequency, your review dates are scheduled for the end of every second week throughout your training period.


## ❓ FAQ

**Q: How do I start my surfing goal plan?**
You can use the `generate_goal_roadmap` tool by providing your current skill level, what you want to achieve, and your planned timeline.

**Q: Can I check if my surfing goals are realistic?**
Yes, the `evaluate_goal_feasibility` tool analyzes your aspiration against your current proficiency and available time to provide a feasibility assessment.

**Q: How do I track my progress?**
Use the `get_goal_metrics` tool with a specific goal ID to retrieve quantifiable measurement criteria for your progress.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/surf-goal-framework](https://vinkius.com/en/ai-agent-connect/surf-goal-framework)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surf Goal Framework** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surf-goal-framework` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surf Goal Framework** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surf-goal-framework": {
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
