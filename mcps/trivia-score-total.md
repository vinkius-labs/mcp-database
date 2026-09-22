# Trivia Score Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/trivia-score-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate and aggregate trivia competition scores across multiple rounds.

## Description
This MCP server provides tools to manage trivia competition scoring. You can use `calculate_round_score` to sum points from individual questions, `aggregate_session_total` to find the cumulative score of a session, `validate_score_entry` to ensure scores meet competition rules, and `get_performance_summary` to view high-level metrics like highest and average scores.


## Available Tools (4)
- **aggregate_session_total**: Calculates the cumulative score across multiple trivia rounds
- **get_performance_summary**: Provides a high-level overview of a participant's performance across rounds
- **calculate_round_score**: Calculates the total points earned within a single trivia round
- **validate_score_entry**: Checks if a specific score entry adheres to the competition's scoring rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Trivia Score Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the score for a round where the question points were 10, 5, and 15."

**🤖 AI Agent:**
> The total round score is 30.

---

**👤 You:**
> "What is the total session score if the round scores were 20, 30, and 25?"

**🤖 AI Agent:**
> The total session score is 75.

---

**👤 You:**
> "Is a score of -5 valid?"

**🤖 AI Agent:**
> No, the score is invalid because scores must be non-negative.


## ❓ FAQ

**Q: How do I calculate the total for a single round?**
Use the `calculate_round_score` tool by providing an array of numbers representing the points for each question.

**Q: Can I validate if a score is legal?**
Yes, the `validate_score_entry` tool checks if a score is a non-negative number according to competition rules.

**Q: How can I see a summary of all rounds?**
The `get_performance_summary` tool provides the highest, lowest, and average scores from a list of round scores.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/trivia-score-total](https://vinkius.com/en/ai-agent-connect/trivia-score-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Trivia Score Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `trivia-score-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Trivia Score Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "trivia-score-total": {
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
