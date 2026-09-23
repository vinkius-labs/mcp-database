# Quiz Average Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/quiz-average-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Calculate and analyze student quiz performance metrics.

## Description
This MCP server provides tools to analyze student quiz performance. Use `get_average_score` to find the mean of multiple scores, `get_performance_spread` to determine the range between minimum and maximum values, `evaluate_passing_status` to check if a score meets a specific threshold, and `get_tier_classification` to assign qualitative performance categories.


## Available Tools (4)
- **evaluate_passing_status**: Checks if a calculated average meets a specific requirement
- **get_average_score**: Calculates the mean score from a provided list of quiz results
- **get_performance_spread**: Determines the range and distribution of scores
- **get_tier_classification**: Maps a score to a qualitative performance category


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Quiz Average Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the average of these quiz scores: 85, 90, 78, 92, 88?"

**🤖 AI Agent:**
> The average score is 86.6.

---

**👤 You:**
> "If the passing threshold is 70, did a score of 65 pass?"

**🤖 AI Agent:**
> No, a score of 65 is below the threshold of 70.

---

**👤 You:**
> "What is the score range for 50, 60, 70, 80, 90?"

**🤖 AI Agent:**
> The score range is 40 (from a minimum of 50 to a maximum of 90).


## ❓ FAQ

**Q: How do I calculate the mean score?**
You can use the `get_average_score` tool by providing a list of numeric scores.

**Q: Can I check if a student passed a quiz?**
Yes, use `evaluate_passing_status` with the average score and the required threshold.

**Q: How is performance categorized?**
The `get_tier_classification` tool maps scores to qualitative tiers like Mastery or Needs Improvement.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/quiz-average-analytics](https://vinkius.com/en/ai-agent-connect/quiz-average-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Quiz Average Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `quiz-average-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Quiz Average Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "quiz-average-analytics": {
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
