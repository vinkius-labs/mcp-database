# Venture Fund DPI Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-fund-dpi-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate DPI, TVPI, and RVPI ratios for venture capital funds.

## Description
This MCP server provides specialized financial tools for private equity and venture capital analysis. It allows AI agents to calculate the Distributed to Paid-In (DPI) ratio, evaluate performance against industry benchmarks, and assess total value impact using TVPI and RVPI metrics. Use `calculate_current_dpi` for core ratios, `get_vintage_performance` to compare fund cohorts, `compareToBenchmark` to check performance tiers, and `calculate_total_value_impact` for a complete view of realized and unrealized value.


## Available Tools (4)
- **compare_to_benchmark**: Evaluates a fund's performance against industry standard benchmarks
- **get_vintage_performance**: Aggregates and compares DPI ratios across different fund vintages
- **calculate_current_dpi**: Calculates the core DPI ratio for a specific fund based on its current financial state
- **calculate_total_value_impact**: Provides a holistic view of value by combining DPI with the remaining NAV


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Fund DPI Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the DPI for a fund with $50M in distributions and $40M paid-in capital?"

**🤖 AI Agent:**
> The DPI for this fund is 1.25.

---

**👤 You:**
> "Compare a fund with 1.5 DPI and 6 years of age against the growth benchmark."

**🤖 AI Agent:**
> The fund is outperforming the growth benchmark.

---

**👤 You:**
> "Calculate the total value impact for $30M distributions, $20M NAV, and $40M paid-in."

**🤖 AI Agent:**
> The DPI is 0.75, the TVPI is 1.25, and the RVPI is 0.5.


## ❓ FAQ

**Q: How is DPI calculated?**
DPI is calculated by dividing the total distributions (cash and in-kind) by the total paid-in capital. The `calculate_current_dpi` tool also accounts for recycled capital to ensure accuracy.

**Q: Can I compare my fund to industry standards?**
Yes, you can use the `compareToBenchmark` tool to evaluate if a fund is outperforming, at-benchmark, or underperforming based on its age and tier.

**Q: What is the difference between DPI and TVPI?**
DPI measures realized value (distributions), while TVPI (Total Value to Paid-In) measures both realized and unrealized value (distributions plus NAV). Use `calculate_total_value_impact` to see both.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-fund-dpi-calculator](https://vinkius.com/en/ai-agent-connect/venture-fund-dpi-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Fund DPI Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-fund-dpi-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Fund DPI Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-fund-dpi-calculator": {
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
