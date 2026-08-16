# Reasoning Step Word Count Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/reasoning-step-word-count-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Analyzes ReAct traces to measure reasoning depth and identify zero-shot behavior.

## Description
This MCP server provides tools to evaluate the quality of the ReAct (Reasoning + Acting) framework. It calculates the verbosity ratio between the 'Thought' and 'Action' phases of an LLM trace. By using `analyze_trace_verbosity`, you can detect zero-shot behavior where the thought block is too brief. You can also use `aggregate_trace_metrics` to summarize reasoning patterns across entire traces or `identify_high_verbosity_steps` to find moments of deep cognitive effort.


## Available Tools (3)
- **analyze_trace_verbosity**: 
- **identify_high_verbosity_steps**: 
- **aggregate_trace_metrics**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reasoning Step Word Count Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this ReAct step: Thought: 'I need to find the weather.' Action: 'get_weather(city="London")'"

**🤖 AI Agent:**
> {"thoughtWordCount": 6, "actionWordCount": 3, "verbosityRatio": 2.0, "isZeroShot": true}

---

**👤 You:**
> "Summarize these steps: [{'thoughtWordCount': 20, 'actionWordCount': 5, 'verbosityRatio': 4.0, 'isZeroShot': false}]"

**🤖 AI Agent:**
> {"totalSteps": 1, "averageVerbosityRatio": 4.0, "zeroShotCount": 0, "totalThoughtWords": 20, "totalActionWords": 5}

---

**👤 You:**
> "Find steps with a verbosity ratio higher than 2.0 in this list: [{'thoughtWordCount': 30, 'actionWordCount': 5, 'verbosityRatio': 6.0, 'isZeroShot': false}]"

**🤖 AI Agent:**
> {"highVerbositySteps": [{'thoughtWordCount': 30, 'actionWordCount': 5, 'verbosityRatio': 6.0, 'isZeroShot': false}], "count": 1}


## ❓ FAQ

**Q: What is a zero-shot indicator in this context?**
A zero-shot indicator is triggered when the `analyze_trace_verbosity` tool finds that the thought block contains fewer than 10 words, suggesting the model skipped detailed reasoning.

**Q: How is the verbosity ratio calculated?**
The verbosity ratio is the total word count of the thought block divided by the total word count of the action block.

**Q: Can I summarize multiple steps at once?**
Yes, you can use `aggregate_trace_metrics` to get a high-level summary of total steps, average verbosity, and zero-shot counts for a collection of analysis results.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/reasoning-step-word-count-analyzer](https://vinkius.com/ai-agent-connect/reasoning-step-word-count-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reasoning Step Word Count Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reasoning-step-word-count-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reasoning Step Word Count Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reasoning-step-word-count-analyzer": {
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
