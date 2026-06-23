# Startup Health Score MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/startup-health-score)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Quantify startup operational health (0-100) across Finance, Product, Growth, Team, and Market dimensions using stage-specific benchmarks.

## Description
The Startup Health Score MCP provides a multi-dimensional analytical engine to evaluate business stability and growth potential. By benchmarking key performance indicators (KPIs) against stage-specific targets--from Pre-seed to Series B--it identifies critical risks and operational strengths. Use `retrieve_stage_benchmarks` to find ideal thresholds, `evaluate_dimension_performance` to compare actual metrics like Runway or CAC against those targets, and `generate_comprehensive_health_report` to produce a final health score and diagnostic summary.


## Available Tools (3)
- **evaluate_dimension_performance**: Calculates how well a single dimension is performing against targets
- **generate_comprehensive_health_report**: Aggregates all dimensional scores to produce the final health score
- **retrieve_stage_benchmarks**: Provides target ideal values for all metrics based on a specific startup stage


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Startup Health Score** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the target benchmarks for a Seed stage startup?"

**🤖 AI Agent:**
> For the Seed stage, ideal targets include a Runway of at least 18 months, a Burn Multiple below 2.0, and a Retention Rate of over 40%.

---

**👤 You:**
> "My startup is at Series A. Our CAC is $50 and our target is $40. How does this affect our Growth score?"

**🤖 AI Agent:**
> Since your actual CAC ($50) is higher than the Series A target ($40), your Growth dimension score will decrease, reflecting lower capital efficiency in customer acquisition.

---

**👤 You:**
> "Generate a health report for a Series B company with the following scores: Finance: 0.8, Product: 0.9, Growth: 0.4, Team: 0.7, Market: 0.6."

**🤖 AI Agent:**
> Your final health score is 68/100. Status: Stable. Strengths: Product and Finance. Critical Risks: Growth (due to low efficiency in CAC/MoM).


## ❓ FAQ

**Q: How does the health score calculation work?**
The engine evaluates five dimensions: Finance, Product, Growth, Team, and Market. It compares your actual metrics against benchmarks retrieved via `retrieve_stage_benchmarks` for your specific stage (e.g., Series A) to calculate a normalized score.

**Q: What metrics are evaluated?**
The evaluation includes Finance (Runway, Burn Multiple), Product (Retention, NPS), Growth (MoM, CAC), Team (Headcount vs Revenue), and Market (TAM Share).

**Q: Can I use this for different funding stages?**
Yes, the tool uses stage-specific benchmarks for Pre-seed, Seed, Series A, and Series B to ensure the evaluation is contextually accurate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/startup-health-score](https://vinkius.com/mcp/startup-health-score)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Startup Health Score** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `startup-health-score` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Startup Health Score** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "startup-health-score": {
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
