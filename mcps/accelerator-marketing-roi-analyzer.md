# Accelerator Marketing ROI Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-marketing-roi-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Analyze marketing efficiency and ROI for accelerator program pipelines.

## Description
This MCP server provides analytical tools to evaluate the financial impact of marketing activities within an accelerator program. It calculates critical KPIs such as Cost per Application (CPA) and Cost per Accepted Company (CPAC) across paid and organic channels. Use `get_channel_performance` to see granular channel data, `get_aggregate_pipeline_metrics` for total program efficiency, and `get_acquisition_efficiency_ranking` to identify the most cost-effective acquisition paths.


## Available Tools (3)
- **get_aggregate_pipeline_metrics**: 
- **get_acquisition_efficiency_ranking**: 
- **get_channel_performance**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Marketing ROI Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the performance breakdown for these channels: LinkedIn ($5000, 100 apps, 10 accepted), Google ($3000, 50 apps, 5 accepted), and SEO ($0, 40 apps, 2 accepted)."

**🤖 AI Agent:**
> LinkedIn: CPA $50, CPAC $500, ROI 0.2; Google: CPA $60, CPAC $600, ROI 0.16; SEO: CPA $0, CPAC $0, ROI N/A.

---

**👤 You:**
> "What is the total program efficiency for my marketing spend?"

**🤖 AI Agent:**
> The total program spend is $8,000, with 190 total applications and 17 accepted companies. The aggregate cost per application is $42.11.

---

**👤 You:**
> "Which channels are most efficient at getting accepted companies?"

**🤖 AI Agent:**
> The most efficient channel for accepted companies is SEO, followed by LinkedIn and then Google.


## ❓ FAQ

**Q: What metrics can I calculate?**
You can calculate Cost per Application, Cost per Accepted Company, and overall Marketing ROI using tools like `get_channel_performance`.

**Q: How does the tool handle organic vs paid channels?**
The tool distinguishes between paid channels (where spend > 0) and organic channels (where spend is 0) to provide an organic vs paid ratio via `get_aggregate_pipeline_metrics`.

**Q: Can I rank my marketing channels by efficiency?**
Yes, use `get_acquisition_efficiency_ranking` to sort channels by either cost per application or cost per accepted company.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-marketing-roi-analyzer](https://vinkius.com/ai-agent-connect/accelerator-marketing-roi-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Marketing ROI Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-marketing-roi-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Marketing ROI Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-marketing-roi-analyzer": {
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
