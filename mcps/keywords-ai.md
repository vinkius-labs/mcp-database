# Keywords AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/keywords-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Monitor and optimize your LLM API usage with a unified gateway that tracks costs, latency, and model performance across providers.

## Description
Connect your **Keywords AI** account to any AI agent and monitor LLM performance.

### What you can do

- **Request Logs** — List and filter all LLM API calls by model
- **Cost Tracking** — Monitor credit balance and usage statistics
- **Analytics** — View cost trends, latency metrics, and error rates
- **Model Catalog** — Browse available LLM models
- **Team Management** — List users and view activity
- **Alerts** — Review monitoring thresholds


## Available Tools (11)
- **check_keywordsai_status**: Verify API connectivity
- **get_analytics**: Get analytics dashboard
- **get_credits**: Get credit balance
- **get_request**: Get request details
- **get_usage_stats**: Get usage statistics
- **get_user**: Get user details
- **list_alerts**: List monitoring alerts
- **list_models**: List available models
- **list_requests_by_model**: List requests by model
- **list_requests**: List API request logs
- **list_users**: List team users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Keywords AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show my current credit balance."

**🤖 AI Agent:**
> Credit balance: .50 remaining. Usage this month: .80. Top model by cost: GPT-4 (.10).

---

**👤 You:**
> "List all requests using GPT-4."

**🤖 AI Agent:**
> 234 requests using GPT-4 this month. Average latency: 1.2s, average tokens: 850, total cost: .10.

---

**👤 You:**
> "Show analytics dashboard."

**🤖 AI Agent:**
> Analytics summary: 1,234 total requests, .80 total cost, 98.2% success rate, p50 latency 890ms, p99 2.1s.


## ❓ FAQ

**Q: Can my AI track LLM costs?**
Yes. `get_credits` shows your balance, `get_usage_stats` breaks down costs by model and time period.

**Q: Can I filter request logs by model?**
Yes. `list_requests_by_model` returns only requests made to a specific LLM.

**Q: What analytics are available?**
`get_analytics` provides cost trends, latency percentiles, error rates, and token usage over time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/keywords-ai](https://vinkius.com/mcp/keywords-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Keywords AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `keywords-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Keywords AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "keywords-ai": {
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
