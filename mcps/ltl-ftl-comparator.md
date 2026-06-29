# LTL-FTL Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ltl-ftl-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Logistics decision engine to compare LTL and FTL shipment costs, risks, and break-even points.

## Description
The LTL-FTL Comparator is a specialized logistics tool designed to optimize shipping decisions. By analyzing weight, volume (CBM), cargo value, and delivery deadlines, it provides precise comparisons between Less than Truckload (LTL) and Full Truckload (FTL) modes. Use `calculate_ltl_metrics` to determine chargeable weight and cost per kg, or `calculate_ftl_metrics` to assess truck capacity utilization. The engine also identifies the exact tonnage break-even point using `find_break_even_threshold`, helping managers decide when a dedicated truck becomes more economical than consolidated shipments. For complex scenarios involving risk tolerance and time constraints, `get_shipment_recommendation` provides a data-driven decision based on cost, speed, and cargo safety.


## Available Tools (4)
- **find_break_even_threshold**: Find the weight threshold where FTL becomes cheaper than LTL
- **calculate_ftl_metrics**: Calculate FTL shipment metrics
- **calculate_ltl_metrics**: Calculate LTL shipment metrics
- **get_shipment_recommendation**: Get a shipment mode recommendation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LTL-FTL Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a shipment of 500kg and 2 CBM with a value of $1000. What are the LTL metrics?"

**🤖 AI Agent:**
> For your 500kg, 2 CBM shipment, the chargeable weight is 666 kg (based on a 333 factor). The total LTL cost is $1,100.00, with a cost per kg of $2.20.

---

**👤 You:**
> "Calculate FTL metrics for 5000kg and 15 CBM in a truck with 10000kg and 30 CBM capacity. Cargo value is $5000."

**🤖 AI Agent:**
> The FTL shipment cost is $1,250.00, with a capacity utilization of 50% for weight and 50% for volume.

---

**👤 You:**
> "Should I use LTL or FTL for a 2000kg shipment that needs to arrive in 12 hours with low risk tolerance?"

**🤖 AI Agent:**
> The recommended mode is FTL. Although LTL might be cheaper, the strict 12-hour deadline and your low risk tolerance for cargo damage make FTL the necessary choice to ensure safety and speed.


## ❓ FAQ

**Q: How is chargeable weight calculated in LTL?**
The engine calculates volumetric weight by multiplying the volume (CBM) by a volumetric factor. The `calculate_ltl_metrics` tool then selects the higher value between the actual weight and this volumetric weight as the chargeable weight.

**Q: What is the break-even threshold?**
The break-even threshold is the specific weight (in kg) where the total cost of an FTL shipment becomes lower than the cost of an LTL shipment. You can find this using the `find_break_even_threshold` tool.

**Q: Does the recommendation consider cargo risk?**
Yes. The `get_shipment_recommendation` tool evaluates your specified `riskTolerance`. For example, if you have low risk tolerance and high cargo value, it may recommend FTL to minimize handling points.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ltl-ftl-comparator](https://vinkius.com/mcp/ltl-ftl-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LTL-FTL Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ltl-ftl-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LTL-FTL Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ltl-ftl-comparator": {
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
