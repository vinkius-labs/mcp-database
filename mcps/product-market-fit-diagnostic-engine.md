# Product-Market Fit Diagnostic Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/product-market-fit-diagnostic-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [product-management](../categories/product-management.md)

Evaluates product maturity and market resonance using retention, sentiment, and growth signals.

## Description
This MCP server provides a diagnostic engine to evaluate how well a product satisfies market needs. It synthesizes key metrics like retention curves, the Sean Ellis test, and NPS into a unified readiness score. Use `calculate_pmf_score` to get a quantitative health assessment, `analyze_retention_health` to check if your user base is stabilizing, `evaluate_growth_efficiency` to measure market pull, and `get_improvement_priorities` to identify critical business interventions.


## Available Tools (4)
- **analyze_retention_health**: Evaluates whether the user base is stabilizing or leaking
- **calculate_pmf_score**: Provides the primary quantitative assessment of product health
- **evaluate_growth_efficiency**: Determines if growth is sustainable and driven by market demand
- **get_improvement_priorities**: Identifies specific areas of the business model that require intervention to increase PMF


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Product-Market Fit Diagnostic Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my PMF score with 30% retention, 40 NPS, 10% organic growth, 5% referral rate, and 35% Sean Ellis score."

**🤖 AI Agent:**
> Your PMF score is 42, indicating a Foundational readiness level with a moderate confidence rating.

---

**👤 You:**
> "Analyze this retention data: 100, 50, 30, 25, 22, 21."

**🤖 AI Agent:**
> The retention curve is flattened, indicating a stable user base with a Strong health status.

---

**👤 You:**
> "Is my growth efficient with 15% organic growth, 10% referral rate, and $5.00 paid acquisition cost?"

**🤖 AI Agent:**
> Your growth efficiency is High, with a viral coefficient of 0.25 and a sustainability score of 75.


## ❓ FAQ

**Q: How is the PMF score calculated?**
The score is a weighted composite of user retention, NPS, organic growth, referral rates, and the Sean Ellis 'very disappointed' percentage via the `calculate_pmf_score` tool.

**Q: Can I analyze my retention curve?**
Yes, use `analyze_retention_health` by providing a sequence of retention percentages to determine if your cohort is stabilizing or leaking.

**Q: What are improvement priorities?**
The `get_improvement_priorities` tool identifies the most critical areas for intervention based on your current metrics deviation from ideal benchmarks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/product-market-fit-diagnostic-engine](https://vinkius.com/ai-agent-connect/product-market-fit-diagnostic-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Product-Market Fit Diagnostic Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `product-market-fit-diagnostic-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Product-Market Fit Diagnostic Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "product-market-fit-diagnostic-engine": {
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
