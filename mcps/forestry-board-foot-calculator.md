# Forestry Board Foot Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/forestry-board-foot-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Deterministic timber volume and basal area calculator for forestry professionals.

## Description
This MCP server provides precise timber volume and basal area calculations for forestry management. It allows users to estimate board foot yields using standard log rules like Doyle, Scribner, and International 1/4-inch. The toolset includes `calculate_log_volume` for individual tree volume, `calculate_basal_area` for cross-sectional area, and `estimate_acreage_yield` to project total timber volume per acre based on sample data. It accounts for natural taper in large-diameter trees to ensure accuracy.


## Available Tools (3)
- **calculate_log_volume**: Calculates the estimated board foot volume of a single tree using a specific log rule
- **estimate_acreage_yield**: Calculates the total merchantable timber volume across a defined area based on a sample
- **calculate_basal_area**: Determines the cross-sectional area of a single tree at breast height


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Forestry Board Foot Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the volume for a tree with 20 inch DBH and 40 feet of merchantable height using the Doyle rule."

**🤖 AI Agent:**
> The estimated volume for this tree using the Doyle rule is 145 board feet.

---

**👤 You:**
> "What is the basal area for a tree with a 15 inch diameter?"

**🤖 AI Agent:**
> The basal area for a tree with a 15 inch diameter is 1.227 square feet.

---

**👤 You:**
> "Estimate the yield per acre for a sample where the total volume is 500 board feet, BAF is 2, total basal area is 100 sq ft, and sample size is 0.1 acres."

**🤖 AI Agent:**
> The estimated total timber volume is 5,000 board feet per acre.


## ❓ FAQ

**Q: Which log rules are supported?**
The tool supports Doyle, Scribner, and International 1/4-inch log rules.

**Q: How does the tool handle large trees?**
The `calculate_log_volume` tool applies taper deductions for large diameters to account for natural stem narrowing.

**Q: Can I estimate yield per acre?**
Yes, use the `estimate_acreage_yield` tool by providing tree volumes, the BAF used, total basal area sampled, and the sample acreage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/forestry-board-foot-calculator](https://vinkius.com/ai-agent-connect/forestry-board-foot-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Forestry Board Foot Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `forestry-board-foot-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Forestry Board Foot Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "forestry-board-foot-calculator": {
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
