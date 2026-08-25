# Accelerator Interview Scoring MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-interview-scoring)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze interview scoring consistency and identify calibration needs to ensure fair candidate evaluations.

## Description
This MCP server provides tools to evaluate the quality and uniformity of candidate evaluations. It helps organizations ensure that candidate scores reflect merit rather than interviewer subjectivity. Use `get_scoring_consistency` to measure agreement among interviewers, `evaluate_calibration_needs` to identify when standards need alignment, and `calculate_score_adjustments` to mitigate interviewer bias through mathematical corrections.


## Available Tools (3)
- **evaluate_calibration_needs**: Answers "Which interviewers or candidates require a calibration session to align standards?"
- **get_scoring_consistency**: Answers "How much do our interviewers agree on candidate evaluations?"
- **calculate_score_adjustments**: Answers "How should we adjust individual scores to compensate for interviewer bias?"


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Interview Scoring** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much do our interviewers agree on these scores: [8, 7, 9, 8] with a reliability of 0.8?"

**🤖 AI Agent:**
> The scoring consistency is high, indicating strong agreement among the interviewers.

---

**👤 You:**
> "Do we need a calibration session? The variance is 0.5, training level is 0.7, and history is []."

**🤖 AI Agent:**
> No, current variance is within acceptable limits for the current training level.

---

**👤 You:**
> "Adjust these scores [7, 9] for a bias coefficient of -0.2 and training effect of 0.1."

**🤖 AI Agent:**
> The adjusted scores are [7.2, 8.8].


## ❓ FAQ

**Q: How does this tool help reduce hiring bias?**
It uses `calculate_score_adjustments` to apply mathematical corrections to scores from lenient or harsh interviewers, ensuring a more neutral evaluation.

**Q: When should we run a calibration session?**
You can use `evaluate_calibration_needs` to determine if current score variance requires a session based on your interviewer training levels.

**Q: What is scoring consistency?**
It is a measure of how closely multiple interviewers agree on the same candidate, which can be calculated using `get_scoring_consistency`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-interview-scoring](https://vinkius.com/ai-agent-connect/accelerator-interview-scoring)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Interview Scoring** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-interview-scoring` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Interview Scoring** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-interview-scoring": {
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
