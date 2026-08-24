# Accelerator Session Effectiveness Evaluator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-session-effectiveness-evaluator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Compares online vs offline session effectiveness and calculates optimal delivery mixes.

## Description
This MCP server provides decision-support tools for accelerator programs to evaluate delivery modes. Use `compare_delivery_modes` to determine which mode is more cost-effective based on engagement and outcomes. Use `calculate_optimal_mix` to find the ideal balance of online and offline sessions within a budget. You can also use `evaluate_session_suitability` to decide if a specific topic is better suited for digital or in-person delivery.


## Available Tools (3)
- **compare_delivery_modes**: Compares the effectiveness and cost-effectiveness of online versus offline delivery modes
- **evaluate_session_suitability**: Evaluates if a specific topic is better suited for online or offline delivery
- **calculate_optimal_mix**: Calculates the ideal distribution of online and offline sessions to maximize impact within a budget


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Session Effectiveness Evaluator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which mode is better: online with 80% attendance and 7 engagement, or offline with 60% attendance and 9 engagement? Both cost $500."

**🤖 AI Agent:**
> The offline mode is the winner due to higher cost-effectiveness driven by the superior engagement score.

---

**👤 You:**
> "What is the best mix for a $5000 budget if participants prefer online (0.8) and the content is highly technical (0.9)?"

**🤖 AI Agent:**
> The optimal mix suggests a higher proportion of online sessions to maximize the budget while respecting participant preference and technical suitability.

---

**👤 You:**
> "Is a hands-on coding workshop better online or offline? It requires high interaction (9) and low tech dependency (2)."

**🤖 AI Agent:**
> The recommended mode is offline because the high interaction requirement outweighs the low technical dependency.


## ❓ FAQ

**Q: How does the tool determine the winner between online and offline modes?**
The `compare_delivery_modes` tool calculates the effectiveness ratio (attendance, engagement, and outcome correlation) and divides it by the cost per session to find the most cost-effective mode.

**Q: Can I plan a full program budget with this tool?**
Yes, by using `calculate_optimal_mix`, you can input your total budget and receive a recommendation for the number of online and offline sessions that maximizes impact.

**Q: How is content suitability determined?**
The `evaluate_session_suitability` tool analyzes the interaction requirements and technical dependencies of a topic to recommend the best delivery mode.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-session-effectiveness-evaluator](https://vinkius.com/ai-agent-connect/accelerator-session-effectiveness-evaluator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Session Effectiveness Evaluator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-session-effectiveness-evaluator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Session Effectiveness Evaluator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-session-effectiveness-evaluator": {
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
