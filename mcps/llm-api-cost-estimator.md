# LLM API Cost Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/llm-api-cost-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Calculate exact API costs and track session budgets for LLM workflows.

## Description
Prevent budget overruns in agentic workflows by calculating precise token costs. This MCP provides tools to determine the cost of individual LLM calls and track cumulative spending across entire sessions. Use `estimate_single_call` to find the cost of a specific request, or `track_session_usage` to monitor your total spend against a set budget. It supports major providers like OpenAI, Anthropic, and Google with a deterministic pricing matrix.


## Available Tools (3)
- **estimate_single_call**: Calculates the exact cost of a single API request based on token counts and model type
- **track_session_usage**: Updates the running total of costs for a specific workflow and checks against a defined budget
- **get_pricing_catalog**: Retrieves the current deterministic pricing rates for all supported models


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LLM API Cost Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will it cost to run a GPT-4o request with 500 input tokens and 200 output tokens?"

**🤖 AI Agent:**
> The total cost for that request is $0.005.

---

**👤 You:**
> "I have a budget of $5.00 for this session. I just spent $0.50. How much budget is left?"

**🤖 AI Agent:**
> You have $4.50 remaining in your budget.

---

**👤 You:**
> "What are the current pricing rates for Claude 3.5 Sonnet?"

**🤖 AI Agent:**
> Claude 3.5 Sonnet has an input rate of $3.00 per 1M tokens and an output rate of $15.00 per 1M tokens.


## ❓ FAQ

**Q: How do I calculate the cost of a single request?**
You can use the `estimate_single_call` tool by providing the model ID and the number of input and output tokens.

**Q: Can I track my total spending for a specific agent run?**
Yes, use `track_session_usage` with a unique session ID to maintain a running total of costs and monitor your remaining budget.

**Q: Which models are supported?**
The tool supports major models from OpenAI, Anthropic, and Google. You can view the full list of supported models using `get_pricing_catalog`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/llm-api-cost-estimator](https://vinkius.com/ai-agent-connect/llm-api-cost-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LLM API Cost Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `llm-api-cost-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LLM API Cost Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "llm-api-cost-estimator": {
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
