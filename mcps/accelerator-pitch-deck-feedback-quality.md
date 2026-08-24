# Accelerator Pitch Deck Feedback Quality MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-pitch-deck-feedback-quality)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Analyze pitch deck improvement velocity and feedback effectiveness.

## Description
This MCP server provides tools to measure the effectiveness of feedback sessions during the pitch deck iteration process. Use `analyze_improvement_velocity` to track how quickly your deck is improving, `find_optimal_feedback_cadence` to identify the ideal number of feedback loops before hitting diminishing returns, and `evaluate_feedback_impact` to determine if feedback is successfully driving investor interest.


## Available Tools (3)
- **analyze_improvement_velocity**: 
- **evaluate_feedback_impact**: 
- **find_optimal_feedback_cadence**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Pitch Deck Feedback Quality** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How fast is my pitch deck improving based on these iterations?"

**🤖 AI Agent:**
> Your pitch deck is showing Rapid improvement with an average quality increase of 12% per iteration.

---

**👤 You:**
> "When should I stop doing feedback sessions to reach a quality score of 85?"

**🤖 AI Agent:**
> You are recommended to complete 5 total feedback sessions to reach your target quality score efficiently.

---

**👤 You:**
> "Is the feedback I'm getting actually helping me get more investor interest?"

**🤖 AI Agent:**
> Yes, the feedback has a high effectiveness score, showing a strong correlation between implemented advice and increased investor interest.


## ❓ FAQ

**Q: How do I track my deck's improvement speed?**
You can use the `analyze_improvement_velocity` tool by providing your iteration data and implementation rate.

**Q: Can I find out when to stop iterating on my pitch?**
Yes, the `find_optimal_feedback_cadence` tool identifies the diminishing returns point where additional feedback provides minimal value.

**Q: How is feedback effectiveness measured?**
The `evaluate_feedback_impact` tool correlates the implementation rate of feedback with subsequent changes in investor interest.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-pitch-deck-feedback-quality](https://vinkius.com/ai-agent-connect/accelerator-pitch-deck-feedback-quality)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Pitch Deck Feedback Quality** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-pitch-deck-feedback-quality` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Pitch Deck Feedback Quality** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-pitch-deck-feedback-quality": {
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
