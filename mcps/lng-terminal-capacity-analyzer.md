# LNG Terminal Capacity Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/lng-terminal-capacity-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Calculate LNG import terminal capacity, throughput, and storage utilization.

## Description
This MCP server provides specialized tools for managing LNG import terminal operations. It allows AI agents to calculate annual throughput, evaluate peak sendout capability, and analyze storage utilization. By using `calculate_annual_throughput`, agents can identify if capacity is limited by supply or infrastructure. The `calculate_peak_sendout_capability` tool helps determine remaining capacity after accounting for truck loading and bunkering, while `calculate_storage_utilization` provides critical projections for inventory management following vessel arrivals.


## Available Tools (4)
- **analyze_terminal_efficiency**: Provides a holistic view of terminal performance across multiple metrics
- **calculate_annual_throughput**: Determines the total volume of LNG the terminal can process in a year
- **calculate_peak_sendout_capability**: Evaluates the terminal's ability to meet maximum demand periods
- **calculate_storage_utilization**: Analyzes how much storage is consumed by different activities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LNG Terminal Capacity Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the annual throughput for a terminal with 500,000 m3 storage, 500,000 m3/day sendout, and vessel arrivals of [100000, 150000, 200000]?"

**🤖 AI Agent:**
> The total annual throughput is 450,000 m3, and the bottleneck is supply.

---

**👤 You:**
> "Calculate the available peak sendout if the max sendout is 1000 m3/h, truck loading is 100 m3/h, and bunkering is 50 m3/h."

**🤖 AI Agent:**
> The available peak sendout is 850 m3/h.

---

**👤 You:**
> "What will the storage utilization be if I have 50,000 m3 in a 100,000 m3 tank and a vessel of 40,000 m3 arrives?"

**🤖 AI Agent:**
> The utilization is 50%, and the projected volume after arrival will be 90,000 m3.


## ❓ FAQ

**Q: How can I determine if my terminal is supply-constrained?**
You can use the `calculate_annual_throughput` tool. It returns a `bottleneckType` which will explicitly state if the capacity is limited by 'supply' (vessel arrivals) or 'infrastructure' (sendout rate).

**Q: Does this tool account for truck loading and bunkering?**
Yes. The `calculate_peak_sendout_capability` tool allows you to input truck and bunkering rates to find the remaining available peak sendout for consumer demand.

**Q: Can I project storage levels after a vessel arrives?**
Yes, the `calculate_storage_utilization` tool provides a `projectedPostArrivalVolume` which estimates the volume in tanks immediately after the next scheduled vessel arrival.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/lng-terminal-capacity-analyzer](https://vinkius.com/en/ai-agent-connect/lng-terminal-capacity-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LNG Terminal Capacity Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lng-terminal-capacity-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LNG Terminal Capacity Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lng-terminal-capacity-analyzer": {
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
