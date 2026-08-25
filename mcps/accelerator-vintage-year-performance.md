# Accelerator Vintage Year Performance MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-vintage-year-performance)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze historical performance, benchmark comparisons, and maturity stages for investment cohorts.

## Description
This MCP server provides specialized analytical tools for venture capital and accelerator funds to evaluate investment cohorts. Use `get_vintage_performance_score` to obtain a normalized health metric, `compare_to_benchmarks` to measure performance against historical market data, and `analyze_cohort_maturity` to assess the lifecycle and liquidity profile of a vintage year.


## Available Tools (3)
- **analyze_cohort_maturity**: Assesses the lifecycle status and liquidity profile of an accelerator cohort
- **compare_to_benchmarks**: Evaluates how a specific vintage cohort is performing relative to standard market expectations
- **get_vintage_performance_score**: Provides a single, normalized health score for a specific investment cohort


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Vintage Year Performance** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the performance score for a 2018 vintage with 1.5 DPI, 3.0 TVPI, and 15% IRR?"

**🤖 AI Agent:**
> The performance score for the 2018 vintage is 2.1, which is rated as Average.

---

**👤 You:**
> "How does a 2020 vintage with 2.5 TVPI and 12% IRR compare to benchmarks?"

**🤖 AI Agent:**
> The 2020 vintage is performing 15% above the historical benchmark and is positioned in the Top Quartile.

---

**👤 You:**
> "Analyze the maturity of a cohort with 50 companies, 5 exits, 40 active, and 0.2 DPI."

**🤖 AI Agent:**
> The cohort is in the Early Stage with a low liquidity profile. The expected next phase is increased exit activity.


## ❓ FAQ

**Q: What is a vintage year performance score?**
It is a normalized index that weights realized returns (DPI), unrealized potential (TVPI), and time-adjusted efficiency (IRR) to provide a single health metric for the cohort.

**Q: How does the tool compare my fund to the market?**
By using `compare_to_benchmarks`, the tool evaluates your cohort's TVPI and IRR against hardcoded historical benchmark constants for that specific vintage year.

**Q: Can I determine if my cohort is in the early or mature stage?**
Yes, `analyze_cohort_maturity` assesses the lifecycle status based on the ratio of exits to companies funded and the current DPI.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-vintage-year-performance](https://vinkius.com/ai-agent-connect/accelerator-vintage-year-performance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Vintage Year Performance** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-vintage-year-performance` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Vintage Year Performance** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-vintage-year-performance": {
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
