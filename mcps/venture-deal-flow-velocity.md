# Venture Deal Flow Velocity MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-deal-flow-velocity)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze VC deal flow efficiency, identify pipeline bottlenecks, and forecast investment capacity.

## Description
This MCP server provides specialized analytics for venture capital firms to monitor their investment funnel. It allows AI agents to calculate conversion rates between stages, pinpoint exactly where deals are stalling using `identify_pipeline_bottlenecks`, and project future investment volume with `calculate_capacity_forecast`. Additionally, firms can use `evaluate_quality_adjusted_velocity` to weight their pipeline metrics against deal quality scores, ensuring a realistic view of high-value deal movement.


## Available Tools (4)
- **analyze_funnel_efficiency**: Calculates the conversion rates between every sequential stage in the deal flow funnel
- **calculate_capacity_forecast**: Estimates how many closed deals a firm can expect to achieve based on current incoming volume and conversion efficiencies
- **evaluate_quality_adjusted_velocity**: Adjusts standard funnel metrics by a quality score to provide a more accurate view of "meaningful" deal flow
- **identify_pipeline_bottlenecks**: Pinpoints the specific stage where the deal flow experiences the most significant loss in momentum


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Deal Flow Velocity** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze my deal flow efficiency: 100 deals reviewed, 40 first meetings, 15 follow-up meetings, 5 term sheets, and 2 closed deals."

**🤖 AI Agent:**
> Your conversion rates are: 40% from reviewed to first meetings, 37.5% from first meetings to follow-up meetings, 33.3% from follow-up meetings to term sheets, and 40% from term sheets to closed deals. Your overall conversion rate is 2%.

---

**👤 You:**
> "Where is the bottleneck in my pipeline? I had 50 reviews, 20 first meetings, 5 follow-ups, 2 term sheets, and 1 closed deal."

**🤖 AI Agent:**
> The primary bottleneck is at the follow-up meetings stage, where the conversion rate dropped significantly compared to previous stages.

---

**👤 You:**
> "Based on 200 reviewed deals and my current conversion rates, how many closed deals can I expect?"

**🤖 AI Agent:**
> Based on your current conversion efficiencies, you can expect to achieve 4 closed deals from an incoming volume of 200 reviewed deals.


## ❓ FAQ

**Q: How can I find where my deal flow is getting stuck?**
You can use the `identify_pipeline_bottlenecks` tool to pinpoint the specific stage in your funnel where the most significant loss in momentum occurs.

**Q: Can I project future closed deals based on current performance?**
Yes, the `calculate_capacity_forecast` tool estimates the expected number of closed deals by applying current conversion efficiencies to your incoming deal volume.

**Q: How does deal quality affect the metrics?**
The `evaluate_quality_adjusted_velocity` tool allows you to weight your conversion rates by a quality score (0.0 to 1.0), providing a more accurate view of meaningful deal movement.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-deal-flow-velocity](https://vinkius.com/en/ai-agent-connect/venture-deal-flow-velocity)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Deal Flow Velocity** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-deal-flow-velocity` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Deal Flow Velocity** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-deal-flow-velocity": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
