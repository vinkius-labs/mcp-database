# Funnel Conversion Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/funnel-conversion-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-analytics](../categories/marketing-analytics.md)

Calculate marketing funnel metrics step-by-step and project revenue gains from process improvements.

## Description
Connect this Funnel Conversion Calculator to any AI agent. The funnel is a critical path: Awareness $\to$ Consideration $\to$ Intent $\to$ Purchase. If you don't know where the leaks are, optimizing anything is wasted effort.

**Mechanism:** This toolset provides three core functions:
1. **`calculate_funnel_metrics`**: Establishes your baseline performance by calculating current conversion rates and projected revenue from a starting volume.
2. **`identify_bottleneck`**: Analyzes the baseline results to pinpoint the exact stage (e.g., Consideration) where drop-offs are most severe relative to potential volume, showing you where effort matters most.
3. **`simulate_improvement_impact`**: Allows you to run 'what-if' scenarios. By proposing percentage lifts in specific conversion rates, this function models the resulting additional purchases and the total monetary uplift (projected revenue gain). 

The bridge this provides is direct: It connects raw marketing data volume into actionable financial projections, telling your team exactly how much more money a 1% improvement at the Consideration stage could generate.


## Available Tools (3)
- **identify_bottleneck**: Returns the bottleneck stage name, relative loss percentage, and improvement leverage calculation.

Identify the funnel stage with the highest relative drop-off rate
- **calculate_funnel_metrics**: Calculate funnel conversion metrics across Awareness, Consideration, Intent, and Purchase stages
- **simulate_improvement_impact**: Returns recalculated metrics, overall improvement percentage, additional purchases, and revenue uplift.

Simulate projected financial uplift from targeted funnel stage improvements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Funnel Conversion Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Run the initial analysis. Start with 10,000 leads and assume A->C is 25%, C->I is 30%, and I->P is 70%. The average customer value is $150."

**🤖 AI Agent:**
> The `calculate_funnel_metrics` tool shows a baseline revenue of $3,150. The bottleneck appears to be Consideration, which has the highest relative drop-off.

---

**👤 You:**
> "I want to model an improvement. Let's assume we can improve Consideration by 10% (30% -> 33%) and Intent by 5% (70% -> 73%). Recalculate the impact."

**🤖 AI Agent:**
> Using `simulate_improvement_impact`, we project that these targeted improvements increase total purchases by 450 units, resulting in a $67,500 projected revenue uplift.

---

**👤 You:**
> "Identify the bottleneck for this quarter's data snapshot (A->C: 20%, C->I: 40%, I->P: 65%). Initial volume was 8,000. ARPC is $140."

**🤖 AI Agent:**
> The `identify_bottleneck` tool confirms that the Consideration stage presents the highest relative loss point, requiring immediate focus to maximize return on investment.


## ❓ FAQ

**Q: Does this tool only calculate the conversion rate?**
No. The `calculate_funnel_metrics` function establishes your baseline, but the real power comes from using `identify_bottleneck`. This second tool finds the weakest point, and then you use `simulate_improvement_impact` to quantify the financial value of fixing it.

**Q: Can I test how much revenue an improvement will generate?**
Yes. The `simulate_improvement_impact` tool is designed for this purpose. You input your target percentage lifts, and the function returns a concrete dollar figure of projected revenue uplift.

**Q: What if my funnel has multiple bottlenecks?**
`identify_bottleneck` pinpoints the single highest relative loss area. However, you can run `simulate_improvement_impact` multiple times, focusing on different stages in sequence to model overall improvement across several bottlenecks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/funnel-conversion-calculator](https://vinkius.com/mcp/funnel-conversion-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Funnel Conversion Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `funnel-conversion-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Funnel Conversion Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "funnel-conversion-calculator": {
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
