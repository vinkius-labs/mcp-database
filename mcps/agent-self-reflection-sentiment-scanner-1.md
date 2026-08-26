# Agent Self-Reflection Sentiment Scanner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/agent-self-reflection-sentiment-scanner-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [observability](../categories/observability.md)

Analyzes agent execution logs to detect self-correction markers and measure stability.

## Description
This MCP server provides tools to analyze the 'sentiment' of agentic workflows by tracking deterministic self-correction markers. It identifies Error Recognition Markers (e.g., when an agent realizes a mistake) and Success Markers (e.g., task completion). By using `scan_logs_for_markers`, `calculate_rate`, and `get_summary`, users can calculate the Self-Correction Frequency Rate and assess the stability of agentic loops. It is designed to provide visibility into how often agents identify and fix errors during execution.


## Available Tools (3)
- **calculate_rate**: Computes the statistical frequency of self-corrections relative to the number of loops performed
- **scan_logs**: Analyzes raw log files to identify and count specific markers
- **get_summary**: Aggregates all scanning and calculation data into a single high-level report


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent Self-Reflection Sentiment Scanner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you scan these logs and tell me the correction rate?"

**🤖 AI Agent:**
> The self-correction frequency rate is 0.15, indicating a High stability score for this execution loop.

---

**👤 You:**
> "What was the summary for execution ID 12345?"

**🤖 AI Agent:**
> Execution 12345 had 2 errors detected and 5 successful completions, resulting in a stable execution profile.

---

**👤 You:**
> "How many error markers were found in the provided log content?"

**🤖 AI Agent:**
> A total of 3 error recognition markers were identified in the log content.


## ❓ FAQ

**Q: What are self-correction markers?**
They are specific linguistic phrases like 'I made a mistake' or 'The task is complete' that indicate an agent's internal state transition.

**Q: How is the stability score calculated?**
The stability score is derived from the frequency rate of error recognition markers relative to the total number of completed execution loops.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/agent-self-reflection-sentiment-scanner-1](https://vinkius.com/ai-agent-connect/agent-self-reflection-sentiment-scanner-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agent Self-Reflection Sentiment Scanner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agent-self-reflection-sentiment-scanner-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agent Self-Reflection Sentiment Scanner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agent-self-reflection-sentiment-scanner-1": {
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
