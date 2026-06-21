# Retention Curve Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/retention-curve-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [product-management](../categories/product-management.md)

Analyze cohort retention curves to identify stability versus churn and compare against industry benchmarks.

## Description
The Retention Curve Analyzer is a specialized tool for product managers and growth engineers. It helps you understand user engagement by analyzing retention sequences to determine if your curve is `analyze_retention_trend` (flattening) or `classify_curve_pattern` (declining). By using `verify_benchmark_compliance`, you can compare your actual D1, D7, D30, and D90 metrics against hardcoded industry standards for SaaS, Mobile Gaming, and E-commerce. This allows you to identify 'Smiling Curves' that signify healthy long-term retention versus 'Declining Curves' that indicate high churn risk.


## Available Tools
- **analyze_retention_trend**: Determines if a retention sequence is flattening or declining
- **classify_curve_pattern**: Classifies the retention curve pattern
- **verify_benchmark_compliance**: Compares cohort metrics against industry benchmarks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Retention Curve Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is my retention curve flattening or declining? Here are the values: [100, 50, 30, 25, 22]"

**🤖 AI Agent:**
> The retention curve is Flattening. The recent drop from 25 to 22 is minimal, indicating the curve has reached a plateau.

---

**👤 You:**
> "Check if my SaaS product meets D7 benchmarks. My D1 is 40% and D7 is 20%."

**🤖 AI Agent:**
> The compliance report shows that your D7 metric failed to meet the SaaS benchmark.

---

**👤 You:**
> "What pattern does this sequence represent: [100, 80, 60, 40, 20, 5]?"

**🤖 AI Agent:**
> The pattern is classified as Declining because the sequence shows a continuous downward trend approaching zero.


## ❓ FAQ

**Q: How does the tool determine if a curve is flattening?**
The `analyze_retention_trend` tool examines the change between consecutive values in your retention sequence. If the decrease between recent intervals falls below a specified stability threshold, it is marked as Flattening.

**Q: What categories are supported for benchmarking?**
The tool currently supports benchmarks for SaaS, Mobile Gaming, and E-commerce.

**Q: Can I provide my own stability threshold?**
Yes, when using `analyze_retention_trend`, you can optionally provide a `stabilityThreshold` to define the maximum allowable drop between intervals for a trend to be considered stable.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/retention-curve-analyzer](https://vinkius.com/mcp/retention-curve-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Retention Curve Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `retention-curve-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Retention Curve Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "retention-curve-analyzer": {
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
