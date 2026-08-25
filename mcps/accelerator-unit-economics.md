# Accelerator Unit Economics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-unit-economics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate financial viability and per-company economics for startup accelerators.

## Description
This MCP server provides a specialized toolset for accelerator program managers to evaluate financial sustainability. It allows for precise calculation of individual company returns using `calculate_company_economics`, aggregate cohort-level metrics like sustainability ratios via `calculate_cohort_success_metrics`, and the impact of cross-subsidization through `analyze_subsidization_model`. By modeling the relationship between program costs, equity stakes, and success rates, managers can determine the true cost per successful company and ensure long-term program viability.


## Available Tools (3)
- **calculate_cohort_success_metrics**: Calculates the aggregate impact of success rates and follow-on value on the overall program sustainability
- **calculate_company_economics**: Determines the direct financial relationship between the cost of supporting one company and the expected value of the equity held
- **analyze_subsidization_model**: Evaluates how much surplus value from successful companies is required to cover the costs of unsuccessful companies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Unit Economics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the economics for a company where we spent $50,000, took 5% equity, and expect a $10,000,000 valuation."

**🤖 AI Agent:**
> The equity value is $500,000, resulting in an equity-to-cost ratio of 10.0 and a net gain of $450,000.

---

**👤 You:**
> "What is the cost per successful company if we spend $500,000 on 10 companies with a 20% success rate?"

**🤖 AI Agent:**
> The cost per successful company is $250,000.

---

**👤 You:**
> "Analyze a cohort with a $1,000,000 total cost, 2 expected successful companies, and an average equity value of $600,000 per success."

**🤖 AI Agent:**
> The total surplus is $200,000, and the subsidization requirement to cover unsuccessful companies is $0, as the surplus covers the costs.


## ❓ FAQ

**Q: How do I calculate the return on a single startup?**
You can use the `calculate_company_economics` tool. Provide the cost spent on the company, the equity percentage held, and the expected valuation at exit.

**Q: Can I model the impact of unsuccessful companies on my program?**
Yes, the `analyze_subsidization_model` tool helps you understand how much surplus value from successful companies is needed to cover the costs of those that do not meet targets.

**Q: How is cohort sustainability measured?**
Sustainability is measured using the `calculate_cohort_success_metrics` tool, which calculates the sustainability ratio by comparing the total expected portfolio value to the total cohort cost.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-unit-economics](https://vinkius.com/ai-agent-connect/accelerator-unit-economics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Unit Economics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-unit-economics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Unit Economics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-unit-economics": {
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
