# Bit Selection Optimization MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/bit-selection-optimization)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Select the most efficient drill bit based on geological properties and drilling objectives.

## Description
This MCP server provides specialized decision-support tools for oil and gas drilling operations. It allows AI agents to identify the optimal drill bit by analyzing formation type, compressive strength, and abrasiveness. Using the `select_optimal_bit` tool, agents can determine the best IADC category for a specific formation. Additionally, the `estimate_performance_metrics` tool predicts drilling speed and wear, while `calculate_cost_analysis` determines the financial efficiency via Cost-per-Foot metrics. For complex decisions, `compare_bit_options` provides a side-by-side comparison to identify the most cost-effective configuration.


## Available Tools (4)
- **compare_bit_options**: Provides a side-by-side comparison of two different bit configurations
- **estimate_performance_metrics**: Predicts the expected drilling speed and bit wear characteristics for a selected bit
- **select_optimal_bit**: Recommends the best bit type and IADC category based on geological and objective inputs
- **calculate_cost_analysis**: Determines the financial efficiency of a drilling run using the Cost-per-Foot metric


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bit Selection Optimization** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Recommend a bit for a soft shale formation with a compressive strength of 40 MPa and low abrasiveness for maximum ROP."

**🤖 AI Agent:**
> The recommended bit is a PDC bit with IADC code M123, which is optimized for high ROP in soft formations.

---

**👤 You:**
> "What is the cost-per-foot if the bit costs $50,000, the rig rate is $20,000/hr, the ROP is 50 ft/hr, and the bit life is 20 hours?"

**🤖 AI Agent:**
> The total drilling cost is $450,000 and the cost-per-foot is $450.

---

**👤 You:**
> "Compare a PDC bit (IADC M222) and a Roller Cone bit (IADC 537) for a hard granite formation."

**🤖 AI Agent:**
> The Roller Cone bit (IADC 537) is the winner due to its lower Cost-per-Foot in hard granite formations.


## ❓ FAQ

**Q: How does the tool decide between PDC and Roller Cone bits?**
The `select_optimal_bit` tool evaluates the relationship between the formation's compressive strength and its type to recommend either a PDC bit for shearing or a Roller Cone bit for crushing.

**Q: Can I compare two different bit configurations?**
Yes, you can use the `compare_bit_options` tool to perform a side-by-side comparison of two bit configurations to find the one with the lowest Cost-per-Foot.

**Q: What metrics are included in the cost analysis?**
The `calculate_cost_analysis` tool provides the total drilling cost and the Cost-per-Foot (CPF) based on bit cost, rig rate, and expected ROP.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/bit-selection-optimization](https://vinkius.com/en/ai-agent-connect/bit-selection-optimization)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bit Selection Optimization** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bit-selection-optimization` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bit Selection Optimization** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bit-selection-optimization": {
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
