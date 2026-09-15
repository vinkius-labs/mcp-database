# Email Marketing Effectiveness MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/email-marketing-effectiveness)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Calculate key email marketing KPIs and perform funnel analysis.

## Description
This MCP server provides a specialized analytical engine for email marketing performance. It allows AI agents to calculate critical KPIs such as delivery rate, open rate, CTR, and revenue per email using the `calculate_funnel_metrics` tool. Users can also perform A/B test comparisons with `compare_ab_tests`, analyze audience segmentation via `analyze_segment_performance`, and monitor campaign health using `get_engagement_health`.


## Available Tools (4)
- **analyze_segment_performance**: Identifies how different audience segments are responding to the same email content
- **calculate_funnel_metrics**: Provides a comprehensive breakdown of the campaign performance through the entire engagement funnel
- **compare_ab_tests**: Evaluates the performance difference between two campaign versions to identify a winner
- **get_engagement_health**: Provides a high-level health status of a campaign based on whether rates fall within healthy industry standard thresholds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Email Marketing Effectiveness** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the funnel metrics for a campaign with 1000 sent, 950 delivered, 200 opened, 50 clicked, 10 unsubscribed, and $500 revenue."

**🤖 AI Agent:**
> The campaign metrics are: Delivery Rate: 95%, Open Rate: 21.05%, CTR: 5.26%, Unsubscribe Rate: 1.05%, and Revenue per Email: $0.53.

---

**👤 You:**
> "Compare two versions: Version A has 10% CTR and Version B has 12% CTR."

**🤖 AI Agent:**
> Version B is the winner with a 20% lift in CTR compared to Version A.

---

**👤 You:**
> "Is a campaign with a 98% delivery rate, 25% open rate, 5% CTR, and 0.5% unsubscribe rate healthy?"

**🤖 AI Agent:**
> The campaign status is Healthy.


## ❓ FAQ

**Q: What metrics can I calculate?**
You can calculate delivery rate, open rate, click-through rate (CTR), unsubscribe rate, and revenue per email using the `calculate_funnel_metrics` tool.

**Q: How do I compare two email campaigns?**
Use the `compare_ab_tests` tool by providing the metric data for both versions to identify the winner and the lift percentage.

**Q: Can I check if my campaign is performing well?**
Yes, the `get_engagement_health` tool evaluates your rates against industry standards to provide a status of Healthy, Warning, or Critical.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/email-marketing-effectiveness](https://vinkius.com/en/ai-agent-connect/email-marketing-effectiveness)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Email Marketing Effectiveness** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `email-marketing-effectiveness` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Email Marketing Effectiveness** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "email-marketing-effectiveness": {
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
