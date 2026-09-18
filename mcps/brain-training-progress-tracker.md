# Brain Training Progress Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/brain-training-progress-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze cognitive performance trends, detect plateaus, and receive personalized training advice.

## Description
This MCP server provides a specialized analytics engine for monitoring cognitive performance. It helps users distinguish between genuine skill gains and simple task familiarity using `analyze_practice_effect`. Users can track specific domain trends with `get_skill_progress`, identify when training has stalled using `detect_performance_plateaus`, and receive actionable guidance through `get_training_recommendations` to optimize their mental exercises.


## Available Tools (4)
- **analyze_practice_effect**: Separates genuine cognitive improvement from familiarity gains caused by repeating the same tasks
- **detect_performance_plateaus**: Identifies whether a user has stopped making meaningful gains in specific skills
- **get_skill_progress**: Analyzes the performance trends for a specific cognitive skill over a defined period
- **get_training_recommendations**: Generates personalized training advice based on current progress and plateau status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Brain Training Progress Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How has my memory performance changed over the last month?"

**🤖 AI Agent:**
> Your memory skill shows a positive improvement trend, with average accuracy increasing from 75% to 82% over the last 30 days.

---

**👤 You:**
> "I feel like I'm not improving in my attention exercises. Am I stuck?"

**🤖 AI Agent:**
> A plateau has been detected in your Attention skill. It is recommended to increase your current difficulty level to provide more stimulus.

---

**👤 You:**
> "What is the best way to improve my processing speed right now?"

**🤖 AI Agent:**
> Based on your rapid progress, you should increase your training frequency to maintain momentum.


## ❓ FAQ

**Q: How does the system distinguish between real skill gain and task familiarity?**
The `analyze_practice_effect` tool calculates skill gain by weighting performance against difficulty increases, while familiarity gain is measured by improvements when difficulty remains constant.

**Q: What should I do if I am stuck at the same performance level?**
You can use `detect_performance_plateaus` to confirm if you have reached a plateau, and then use `get_training_recommendations` to receive advice on adjusting difficulty or frequency.

**Q: Can I track progress for specific cognitive domains?**
Yes, the `get_skill_progress` tool allows you to analyze performance trends for specific categories like Memory or Attention over a defined period.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/brain-training-progress-tracker](https://vinkius.com/en/ai-agent-connect/brain-training-progress-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Brain Training Progress Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `brain-training-progress-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Brain Training Progress Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "brain-training-progress-tracker": {
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
