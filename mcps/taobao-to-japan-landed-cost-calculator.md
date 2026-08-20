# Taobao to Japan Landed Cost Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/taobao-to-japan-landed-cost-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate exact landed costs for China-to-Japan shipments, including volumetric weight and customs duties.

## Description
This MCP server provides deterministic calculations for cross-border e-commerce shipments from China to Japan. It handles the complexities of logistics and taxation by providing tools to determine billable weight via `calculate_shipping_details`, calculate the final total in Yen using `calculate_landed_cost_jpy`, and analyze package density with `get_weight_comparison`.


## Available Tools (3)
- **calculate_landed_cost_jpy**: Calculates the final total cost in Japanese Yen, including taxes and duties
- **calculate_shipping_details**: Determines the weight-based shipping cost in RMB
- **get_weight_comparison**: Answers if a package is being charged primarily for its size (volumetric) or its mass (actual)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Taobao to Japan Landed Cost Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the shipping cost for a 2kg package with dimensions 30x30x30 cm and a shipping rate of 15 RMB/kg."

**🤖 AI Agent:**
> The volumetric weight is 3.375 kg, making the billable weight 3.375 kg. At 15 RMB/kg, the shipping cost is 50.625 RMB.

---

**👤 You:**
> "What is the total landed cost for an item priced at 5000 RMB with 50 RMB shipping, an exchange rate of 20 JPY/RMB, and 10% tax?"

**🤖 AI Agent:**
> The total landed cost is 115,500 JPY.

---

**👤 You:**
> "Is a 5kg package with dimensions 50x50x50 cm volumetric heavy?"

**🤖 AI Agent:**
> Yes, the volumetric weight is 15.625 kg, which is significantly higher than the actual weight of 5 kg.


## ❓ FAQ

**Q: How is volumetric weight calculated?**
Volumetric weight is calculated by multiplying the length, width, and height of the package in centimeters and dividing the result by 8000.

**Q: When is Japan customs duty applied?**
Customs duty is applied if the converted value of the goods exceeds 10,000 JPY.

**Q: Can I compare actual weight vs volumetric weight?**
Yes, you can use the `get_weight_comparison` tool to see if your package is being charged based on its physical mass or its volume.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/taobao-to-japan-landed-cost-calculator](https://vinkius.com/ai-agent-connect/taobao-to-japan-landed-cost-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Taobao to Japan Landed Cost Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `taobao-to-japan-landed-cost-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Taobao to Japan Landed Cost Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "taobao-to-japan-landed-cost-calculator": {
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
