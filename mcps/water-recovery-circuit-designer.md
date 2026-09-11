# Water Recovery Circuit Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/water-recovery-circuit-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Models water flow and recycling efficiency for industrial processing plants.

## Description
This MCP server provides engineering tools to model water balance and optimize recycling rates in industrial processing plants. It allows users to calculate necessary volumes for thickener overflow, tailings reclaim, and fresh water makeup. Use `calculate_water_balance` to determine water distribution, `validate_quality_compliance` to ensure recycled water meets purity standards, `simulate_recovery_efficiency` to test different recycle targets, and `optimize_makeup_reduction` to find the maximum possible recycling capacity.


## Available Tools (4)
- **calculate_water_balance**: Determines the necessary volumes of thickener overflow, tailings reclaim, and fresh water makeup to meet a specific demand and recycle target
- **optimize_makeup_reduction**: Identifies the maximum possible recycle rate given the physical constraints of the plant's water recovery infrastructure
- **simulate_recovery_efficiency**: Analyzes how varying the recycle target affects the required fresh water makeup and the reliance on different water sources
- **validate_quality_compliance**: Checks if the available recycled water sources meet the specific purity requirements of the process


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Water Recovery Circuit Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the water balance for a plant needing 1000m3 of water with a 60% recycle target, having 400m3 of thickener overflow and 300m3 of tailings reclaim available."

**🤖 AI Agent:**
> The water balance results are: 400m3 of thickener overflow used, 200m3 of tailings reclaim used, and 400m3 of fresh water makeup required to meet the 1000m3 demand, achieving a 60% recycle rate.

---

**👤 You:**
> "Is the water compliant if the required level is PROCESS_GRADE, thickener is ULTRA_PURE, and tailings is RECLAIM_GRADE?"

**🤖 AI Agent:**
> Yes, the water is compliant because the thickener overflow meets the PROCESS_GRADE requirement.

---

**👤 You:**
> "What is the maximum possible recycle rate for a 500m3 demand with 200m3 thickener overflow and 200m3 tailings reclaim available?"

**🤖 AI Agent:**
> The maximum possible recycle rate is 80%, with a maximum recycled volume of 400m3 and a minimum fresh water makeup of 100m3.


## ❓ FAQ

**Q: How do I calculate the required fresh water makeup?**
You can use the `calculate_water_balance` tool by providing the total process water demand, the desired recycle target, and the available volumes from thickener overflow and tailings reclaim.

**Q: Can I check if my recycled water is clean enough for my process?**
Yes, the `validate_quality_compliance` tool compares the quality tiers of your available water sources against your required process quality level.

**Q: How can I find the maximum possible recycling rate?**
Use the `optimize_makeup_reduction` tool to identify the maximum recycle rate and minimum fresh water makeup based on your plant's physical constraints.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/water-recovery-circuit-designer](https://vinkius.com/en/ai-agent-connect/water-recovery-circuit-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Water Recovery Circuit Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `water-recovery-circuit-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Water Recovery Circuit Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "water-recovery-circuit-designer": {
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
