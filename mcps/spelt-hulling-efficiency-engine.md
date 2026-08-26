# Spelt Hulling Efficiency Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/spelt-hulling-efficiency-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate dehulling yield, kernel breakage, and processing economics for spelt grain.

## Description
This MCP server provides a specialized calculation engine for assessing the efficiency, yield, and economic viability of dehulling spelt grain. It uses mechanical dehulling models to determine how different methods like a stone mill or impact dehuller affect the final product. Users can use `calculate_yield_and_quality` to find expected yields, `compare_dehulling_methods` to evaluate machinery, `estimate_processing_economics` to calculate profit margins, and `optimize_moisture_settings` to find the ideal moisture level for processing.


## Available Tools (4)
- **estimate_processing_economics**: Estimates the total processing cost and resulting product value
- **calculate_yield_and_quality**: Calculates the expected yield and quality of processed spelt
- **compare_dehulling_methods**: Compares different dehulling methods (e.g., stone mill vs. impact dehuller)
- **optimize_moisture_settings**: Finds the ideal moisture level to minimize breakage while maximizing yield


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Spelt Hulling Efficiency Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expected yield and quality for a spelt with 15% hull, size 2.5, thickness 0.1, 12% moisture, and an adherence factor of 1.2?"

**🤖 AI Agent:**
> The expected yield is 82.5% with a broken kernel percentage of 4.2%. The total kernel mass is 82.5 units.

---

**👤 You:**
> "Compare a stone mill and an impact dehuller for grain with 12% hull and an adherence factor of 1.5."

**🤖 AI Agent:**
> The stone mill requires 45 units of energy with 3% breakage and an efficiency rating of 0.85. The impact dehuller requires 65 units of energy with 7% breakage and an efficiency rating of 0.72.

---

**👤 You:**
> "What is the ideal moisture level for a stone mill with 10% hull and 1.3 adherence factor?"

**🤖 AI Agent:**
> The optimal moisture level is 13.5%, which is predicted to yield 88% with only 2.5% breakage.


## ❓ FAQ

**Q: How do I determine the best machinery for my spelt variety?**
You can use the `compare_dehulling_methods` tool. By providing the hull percentage and the adherence factor of your specific variety, the tool will compare energy requirements and predicted breakage for different methods.

**Q: Can I calculate the profit margin for a batch?**
Yes. Use `estimate_processing_economics` after you have obtained your yield data. It calculates the total processing cost and the final product value based on market prices for whole and broken kernels.

**Q: What factors influence the kernel breakage?**
Breakage is primarily influenced by the moisture content, the mechanical method used, and the adherence factor of the grain variety. You can use `optimize_moisture_settings` to find the ideal moisture to minimize this.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/spelt-hulling-efficiency-engine](https://vinkius.com/ai-agent-connect/spelt-hulling-efficiency-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Spelt Hulling Efficiency Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `spelt-hulling-efficiency-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Spelt Hulling Efficiency Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "spelt-hulling-efficiency-engine": {
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
