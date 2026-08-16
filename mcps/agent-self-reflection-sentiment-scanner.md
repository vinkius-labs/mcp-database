# Agent Self-Reflection & Sentiment Scanner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/agent-self-reflection-sentiment-scanner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [observability](../categories/observability.md)

Quantify agent self-correction behavior and sentiment by scanning execution logs for specific error and success markers.

## Description
The Agent Self-Reflection & Sentiment Scanner MCP server provides a specialized engine for analyzing agent execution logs. It identifies deterministic self-correction markers by performing exact phrase matching for error recognition (e.g., 'I made a mistake') and success indicators (e.g., 'The task is complete'). By processing these logs, the server can calculate a self-correction frequency rate per execution loop and determine if an agent's current state is 'Correcting' or 'Proceeding'. Use `analyze_sentiment` to evaluate the emotional tone of log entries and `detect_reflection` to identify instances where the agent expresses internal thoughts or feelings.


## Available Tools (2)
- **analyze_sentiment**: Analyze the sentiment of a given text
- **detect_reflection**: Detect if a text contains self-reflective elements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent Self-Reflection & Sentiment Scanner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this log: 'I made a mistake in the previous step. Let me try again. The task is complete.'"

**🤖 AI Agent:**
> The logs contain error recognition markers ('I made a mistake', 'Let me try again') and a success marker ('The task is complete'). The agent's status is Proceeding.

---

**👤 You:**
> "Is the following text positive or negative: 'I am very happy with the results of this execution.'"

**🤖 AI Agent:**
> The sentiment analysis indicates that the text is positive.

---

**👤 You:**
> "Does this log show self-reflection: 'I am thinking about the best way to approach this problem.'"

**🤖 AI Agent:**
> Yes, the text contains elements of self-reflection as it expresses internal thought processes.


## ❓ FAQ

**Q: How does the scanner identify self-correction?**
The scanner uses exact character-for-character comparison to find predefined error recognition phrases and success markers within your provided execution logs.

**Q: Can I use this to monitor multiple agents?**
Yes, you can pass the raw log text from any agent execution loop into the tools to analyze patterns across different agents and sessions.

**Q: What is the difference between `analyze_sentiment` and `detect_reflection`?**
`analyze_sentiment` evaluates whether text is positive, negative, or neutral, while `detect_reflection` specifically looks for markers of internal thought or self-awareness.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/agent-self-reflection-sentiment-scanner](https://vinkius.com/ai-agent-connect/agent-self-reflection-sentiment-scanner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agent Self-Reflection & Sentiment Scanner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agent-self-reflection-sentiment-scanner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agent Self-Reflection & Sentiment Scanner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agent-self-reflection-sentiment-scanner": {
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
