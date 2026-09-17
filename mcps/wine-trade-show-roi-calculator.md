# Wine Trade Show ROI Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-trade-show-roi-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Calculate financial and strategic ROI for wine industry trade shows.

## Description
This MCP server provides specialized tools for the wine industry to evaluate the effectiveness of trade show participation. It calculates total investment using `get_event_cost_analysis`, assesses lead quality with `get_lead_performance`, quantifies intangible benefits like brand exposure via `get_strategic_value_assessment`, and provides final prioritization through `get_roi_recommendation`.


## Available Tools (4)
- **get_event_cost_analysis**: Calculate total investment for a trade show
- **get_lead_performance**: Assess lead quality and conversion potential
- **get_roi_recommendation**: Final ROI and prioritization
- **get_strategic_value_assessment**: Quantify intangible benefits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Trade Show ROI Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the total cost for a show with a $5000 booth, $2000 travel, $1000 samples, and 20 staff hours at $50/hour."

**🤖 AI Agent:**
> The total investment for the trade show is $9,000.

---

**👤 You:**
> "What is the ROI if I spent $10,000 and gained $25,000 in conversion value and $5,000 in brand value?"

**🤖 AI Agent:**
> The overall ROI is 300%.

---

**👤 You:**
> "I had 50 leads, an average deal value of $1000, and a 10% conversion rate. What is my conversion value?"

**🤖 AI Agent:**
> The total conversion value is $5,000.


## ❓ FAQ

**Q: How does this tool calculate total investment?**
The `get_event_cost_analysis` tool sums booth costs, travel, samples, and staff labor to provide a complete investment figure.

**Q: Can I compare this show to previous ones?**
Yes, the `get_roi_recommendation` tool accepts a list of previous ROIs to determine a prioritization rank.

**Q: Does it account for brand value?**
Yes, `get_strategic_value_assessment` allows you to quantify intangible benefits like brand exposure and relationship building.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-trade-show-roi-calculator](https://vinkius.com/en/ai-agent-connect/wine-trade-show-roi-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Trade Show ROI Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-trade-show-roi-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Trade Show ROI Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-trade-show-roi-calculator": {
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
