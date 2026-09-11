# Reserve Replacement Ratio Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/reserve-replacement-ratio-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate critical petroleum industry metrics like RRR, Reserve Life Index, and F&D costs.

## Description
This MCP server provides specialized tools for petroleum industry professionals to assess reserve sustainability. It calculates the Reserve Replacement Ratio (RRR) to determine if production is being adequately replaced by new discoveries or acquisitions. Users can also predict the longevity of current assets using the Reserve Life Index and evaluate capital efficiency through Finding and Development (F&D) costs. Key tools include `calculate_rrr` for replacement ratios, `calculate_reserve_life` for asset longevity, `calculate_fd_costs` for capital efficiency, and `get_reserve_status` for a comprehensive sustainability overview.


## Available Tools (4)
- **calculate_reserve_life**: Predicts the longevity of current reserve stocks
- **get_reserve_status**: Provides a summary overview of the current reserve health and replacement capability
- **calculate_fd_costs**: Evaluates the capital efficiency of reserve growth
- **calculate_rrr**: Determines the organic and total ability of a company to replace its produced reserves


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reserve Replacement Ratio Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the RRR if production is 500 units, drilling additions are 400, and acquisitions are 150."

**🤖 AI Agent:**
> The total RRR is 1.1 and the organic RRR is 0.8.

---

**👤 You:**
> "What is the reserve life if we have 5000 units of year-end reserves and produce 500 units annually?"

**🤖 AI Agent:**
> The reserve life index is 10 years.

---

**👤 You:**
> "Calculate F&D costs for $2000 spent on 100 units of drilling additions."

**🤖 AI Agent:**
> The finding and development cost is 20 per unit.


## ❓ FAQ

**Q: What is the Reserve Replacement Ratio (RRR)?**
The RRR compares the volume of new reserves added during a period to the volume of reserves produced. A ratio of 1.0 means reserves are being replaced at the same rate they are produced.

**Q: How do I calculate the Reserve Life Index?**
You can use the `calculate_reserve_life` tool by providing the total year-end reserves and the annual production volume.

**Q: Can I distinguish between organic and inorganic additions?**
Yes, the `calculate_rrr` tool provides both the total RRR and the organic RRR, which focuses strictly on drilling additions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/reserve-replacement-ratio-calculator](https://vinkius.com/ai-agent-connect/reserve-replacement-ratio-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reserve Replacement Ratio Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reserve-replacement-ratio-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reserve Replacement Ratio Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reserve-replacement-ratio-calculator": {
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
