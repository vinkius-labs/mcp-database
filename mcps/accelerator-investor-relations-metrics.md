# Accelerator Investor Relations Metrics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-investor-relations-metrics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Quantify investor network quality, conversion funnels, and engagement ROI.

## Description
This MCP server provides specialized analytical tools for startup accelerators to measure the effectiveness of their investor relations. Use `calculate_network_quality` to assess the strategic value of your investor pool, `analyze_conversion_funnel` to identify momentum loss in outreach, and `evaluate_engagement_roi` to determine if engagement efforts yield productive returns. It helps quantify network strength, conversion efficiency, and relationship depth across different investor segments.


## Available Tools (3)
- **analyze_conversion_funnel**: Analyze investor outreach conversion stages
- **calculate_network_quality**: Calculate strategic value of investor network
- **evaluate_engagement_roi**: Evaluate efficiency of engagement efforts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Investor Relations Metrics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the strategic value of my network with 50 investors and an average relationship depth of 0.8?"

**🤖 AI Agent:**
> Your network has a quality score of 85 and is classified as an Elite tier network.

---

**👤 You:**
> "Analyze my conversion funnel: 100 outreach, 20 responses, and 5 term sheets."

**🤖 AI Agent:**
> Your response rate is 20% and your term sheet rate is 25%, resulting in a high funnel efficiency.

---

**👤 You:**
> "Is my engagement ROI efficient with a 0.5 repeat engagement rate, 0.1 term sheet rate, and a quality score of 70?"

**🤖 AI Agent:**
> Your engagement ROI is 3.5, which is rated as High efficiency.


## ❓ FAQ

**Q: How do I measure my network's strategic value?**
You can use the `calculate_network_quality` tool, providing the total investor count and average relationship depth.

**Q: Can I analyze my fundraising conversion stages?**
Yes, the `analyze_conversion_funnel` tool calculates response rates and term sheet rates to show where momentum is lost.

**Q: How is engagement efficiency calculated?**
The `evaluate_engagement_roi` tool calculates efficiency by balancing repeat engagement rates against term sheet generation and network quality.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-investor-relations-metrics](https://vinkius.com/ai-agent-connect/accelerator-investor-relations-metrics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Investor Relations Metrics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-investor-relations-metrics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Investor Relations Metrics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-investor-relations-metrics": {
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
