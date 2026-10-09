# Pottery Clay Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pottery-clay-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utility](../categories/utility.md)

Calculate total clay requirements and estimated waste for ceramic production batches.

## Description
This MCP server provides precise calculations for ceramic production planning. It helps potters determine the exact amount of clay needed for a batch, accounting for both the net weight of the pieces and the anticipated waste from processes like trimming or wedging. Use `get_batch_summary` to get a complete breakdown of net weight, waste weight, and total weight in one call.


## Available Tools (4)
- **get_total_clay_requirement**: Calculates the grand total of clay that must be prepared to complete a batch, including the waste buffer
- **get_waste_estimate**: Calculates the amount of extra clay needed to cover anticipated losses during production
- **get_batch_summary**: Provides a comprehensive breakdown of a production run including net weight, waste, and total weight in a single view
- **get_net_clay_weight**: Determines the exact amount of clay required to produce a specific number of pieces without any waste


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pottery Clay Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much clay do I need for 20 pieces weighing 500g each with a 10% waste factor?"

**🤖 AI Agent:**
> You will need a total of 11,000g of clay. This includes 10,000g of net weight and 1,000g of waste.

---

**👤 You:**
> "Calculate the waste weight for a batch of 50 pieces at 200g each with 5% waste."

**🤖 AI Agent:**
> The estimated waste weight is 50g.

---

**👤 You:**
> "What is the net weight for 12 pieces of 1kg each?"

**🤖 AI Agent:**
> The net weight required is 12kg.


## ❓ FAQ

**Q: How do I calculate the total clay needed for my studio run?**
You can use the `get_total_clay_requirement` tool by providing the number of pieces, the target weight per piece, and your expected waste percentage.

**Q: What is a reasonable waste percentage for pottery?**
Waste percentages vary by scale. For small handcrafted items, a lower percentage might suffice, while industrial scales often require a larger buffer to account for higher loss rates.

**Q: Can I get a full breakdown of my production batch?**
Yes, the `get_batch_summary` tool provides a comprehensive view including net weight, waste weight, and the total weight required.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pottery-clay-calculator](https://vinkius.com/en/ai-agent-connect/pottery-clay-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pottery Clay Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pottery-clay-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pottery Clay Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pottery-clay-calculator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
