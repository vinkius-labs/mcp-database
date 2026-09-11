# Service Contract Negotiation Support MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/service-contract-negotiation-support)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Analyze oilfield service contracts using market benchmarking and performance-based incentive modeling.

## Description
This MCP server provides specialized decision support for oilfield service contract negotiations. It connects AI agents to critical industry data and analytical models to ensure fair pricing and optimized performance. Using `analyze_market_alignment`, agents can compare proposed rates against industry benchmarks to identify savings. The `evaluate_performance_incentives` tool allows for the creation of optimized payout structures tied to KPIs. Additionally, `assess_service_quality_impact` adjusts contract valuations based on technical and HSE performance, while `summarize_negotiation_strategy` synthesizes all findings into a cohesive executive summary for procurement leads.


## Available Tools (4)
- **assess_service_quality_impact**: Quantifies how service quality and HSE compliance should influence the final contract valuation
- **evaluate_performance_incentives**: Recommends an optimal incentive structure to drive desired service outcomes
- **analyze_market_alignment**: Determines how well a proposed contract aligns with current industry pricing and identifies potential savings
- **summarize_negotiation_strategy**: Synthesizes all analysis into a cohesive summary for a procurement lead


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Service Contract Negotiation Support** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare these drilling rates: { "proposedRates": [{"serviceType": "drilling", "rate": 50000}] }, for the category 'drilling'."

**🤖 AI Agent:**
> The fair market rate for drilling is $45,000, representing a $5,000 savings opportunity with an 'Optimal' alignment status.

---

**👤 You:**
> "Recommend an incentive structure for a $100,000 budget where HSE is critical, using metrics: { "metricName": "uptime", "targetValue": 0.95 }, { "metricName": "trir", "targetValue": 0.0 }."

**🤖 AI Agent:**
> The recommended structure allocates $60,000 to HSE compliance and $40,000 to operational uptime, with a total potential payout of $100,000.

---

**👤 You:**
> "Calculate the impact of a 0.9 quality score and 0.8 HSE score on a $1,000,000 contract."

**🤖 AI Agent:**
> The quality adjustment is +$50,000 and the HSE adjustment is +$30,000, resulting in a total adjusted value of $1,080,000.


## ❓ FAQ

**Q: How does the tool identify cost savings?**
The `analyze_market_alignment` tool compares your proposed rates against standardized industry benchmarks to calculate the difference between the proposed price and the fair market rate.

**Q: Can I include safety metrics in the incentive planning?**
Yes. When using `evaluate_performance_incentives`, you can set the `isHseCritical` flag to true, which ensures a significant portion of the budget is tied to HSE compliance and safety metrics.

**Q: How are quality scores applied to the contract value?**
The `assess_service_quality_impact` tool uses normalized technical and HSE scores to calculate adjustments that increase or decrease the base contract value based on performance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/service-contract-negotiation-support](https://vinkius.com/ai-agent-connect/service-contract-negotiation-support)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Service Contract Negotiation Support** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `service-contract-negotiation-support` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Service Contract Negotiation Support** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "service-contract-negotiation-support": {
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
