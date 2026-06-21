# Masonry Quantity Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/masonry-quantity-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate the number of masonry units, mortar volume, and required cement and sand for wall construction.

## Description
This MCP server provides specialized tools for construction estimation. Use `calculate_block_count` to determine the number of blocks needed based on wall area and block type, including waste margins. Use `calculate_mortar_volume` to calculate both bedding and coating mortar volumes. Finally, use `estimate_raw_materials` to convert total mortar volume into specific quantities of cement and sand using a provided mix ratio.


## Available Tools (3)
- **calculate_block_count**: Calculate the number of masonry units required
- **estimate_raw_materials**: Estimate required cement and sand quantities
- **calculate_mortar_volume**: Calculate the required volume of mortar


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Masonry Quantity Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many 9x19x39 hollow blocks do I need for a 50 square meter wall, including 5% waste?"

**🤖 AI Agent:**
> For a 50 square meter wall using hollow_9x19x039 blocks with a 5% waste factor, you will need 657 blocks in total (626 base units plus 31 extra for waste).

---

**👤 You:**
> "Calculate the mortar volume needed for a 20 square meter wall using hollow_14x19x39 blocks with a 0.02m coating thickness."

**🤖 AI Agent:**
> The total mortar volume required is 0.15 cubic meters, consisting of approximately 0.04 cubic meters for bedding and 0.08 cubic meters for the coating.

---

**👤 You:**
> "If I have 2 cubic meters of mortar and a mix ratio of 1:4, how much cement and sand do I need?"

**🤖 AI Agent:**
> For 2 cubic meters of mortar with a 1:4 ratio, you will need approximately 0.53 cubic meters of cement and 2.12 cubic meters of sand.


## ❓ FAQ

**Q: How do I calculate the number of blocks needed for my wall?**
You can use the `calculate_block_count` tool. Provide the total surface area of your wall, the type of block you are using (such as `hollow_9x19x39`), and an optional waste percentage.

**Q: How much mortar do I need for the joints and plastering?**
Use the `calculate_mortar_volume` tool. You will need to provide the wall area, the block type, and the thickness of the coating layer.

**Q: Can I estimate how much cement and sand to buy?**
Yes, by using the `estimate_raw_materials` tool. Once you have the total mortar volume from the previous step, input that volume and your desired mix ratio (e.g., '1:3') to get the required quantities.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/masonry-quantity-calculator](https://vinkius.com/mcp/masonry-quantity-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Masonry Quantity Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `masonry-quantity-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Masonry Quantity Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "masonry-quantity-calculator": {
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
