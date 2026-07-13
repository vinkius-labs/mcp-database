# LLM API Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/llm-api-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Estimate and compare the financial impact of LLM usage across different providers.

## Description
The LLM API Cost Calculator provides a precise way to project expenditures for AI workloads. By analyzing token volumes and provider pricing, you can use `compute_request_cost` to find the exact cost of a single interaction, or `estimate_monthly_spend` to forecast 30-day budgets based on daily request estimates. For multi-model strategies, `compare_providers` identifies the most economical tier for your specific usage profile. Additionally, you can evaluate the financial benefits of prompt caching using `calculate_cache_impact` to see how much savings a high cache hit ratio provides.


## Available Tools (4)
- **compute_request_cost**: Calculates the exact monetary cost of a single LLM API call
- **estimate_monthly_spend**: Projects total expenditure over a 30-day period
- **calculate_cache_impact**: Calculates how prompt caching reduces the cost of a request
- **compare_providers**: Provides a comparative analysis of multiple pricing tiers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LLM API Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much does one request cost with 1000 input tokens and 500 output tokens using the gpt-4o tier?"

**🤖 AI Agent:**
> $0.015

---

**👤 You:**
> "If I make 500 requests per day with 2000 input and 1000 output tokens, what is my monthly spend on the claude-3-haiku tier?"

**🤖 AI Agent:**
> $450.00

---

**👤 You:**
> "Compare the monthly costs for 1000 daily requests (5k input, 2k output) between gpt-4o and claude-3-sonnet."

**🤖 AI Agent:**
> The most cost-effective option is claude-3-sonnet with a projected monthly total of $120.00, compared to gpt-4o at $150.00.


## ❓ FAQ

**Q: How is the monthly cost calculated?**
The tool calculates the cost of a single request based on your input and output tokens, then multiplies that by your estimated daily requests and 30 days.

**Q: Can I compare different models like GPT-4o and Claude?**
Yes, by using the `compare_providers` tool, you can input multiple tier IDs to see a ranked list of costs from cheapest to most expensive.

**Q: Does the calculator account for prompt caching?**
Yes, you can use `calculate_cache_impact` to determine how much a specific cache hit ratio will reduce your input token costs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/llm-api-cost-calculator](https://vinkius.com/mcp/llm-api-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LLM API Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `llm-api-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LLM API Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "llm-api-cost-calculator": {
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
