# Wine Traceability & Lot Tracking MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-traceability-lot-tracking)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Track wine production from grape harvest to bottling with full lineage and recall capabilities.

## Description
This MCP server provides complete traceability for wine production. It allows AI agents to track the lifecycle of wine lots through every stage, including grape harvesting, processing, blending, and bottling. Use `trace_lot_forward` to see all downstream products from a specific lot, `trace_product_backward` to reconstruct a finished product's history, `calculate_recall_scope` to identify all affected products during a contamination event, and `get_lot_genealogy` to inspect the parentage of any specific lot.


## Available Tools (4)
- **trace_lot_forward**: Identifies all downstream products and lots that contain a specific starting lot
- **trace_product_backward**: Reconstructs the entire history of a finished product back to the original grape lots
- **calculate_recall_scope**: Determines every consumer product that must be recalled based on a single contaminated source lot
- **get_lot_genealogy**: Provides a detailed view of how a specific lot was created from its predecessors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Traceability & Lot Tracking** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which products contain grape lot LOT-123?"

**🤖 AI Agent:**
> Grape lot LOT-123 was used in the following products: Cabernet Sauvignon 2022 (Batch A) and the Reserve Blend (Batch B).

---

**👤 You:**
> "Trace the history of product PROD-999."

**🤖 AI Agent:**
> Product PROD-999 originated from grape lots GRAPE-001 and GRAPE-002, which were blended during the fermentation stage in March 2023.

---

**👤 You:**
> "What is the recall scope for contaminated lot CONTAM-456?"

**🤖 AI Agent:**
> The contamination in lot CONTAM-456 affects 3 products: Merlot 2021 (500 bottles), Merlot Reserve (200 bottles), and the Autumn Blend (150 bottles).


## ❓ FAQ

**Q: How can I find all products made from a specific grape lot?**
You can use the `trace_lot_forward` tool by providing the specific lot ID to see all resulting products and intermediate lots.

**Q: What happens if a lot is contaminated?**
Use the `calculate_recall_scope` tool with the problematic lot ID to identify every finished product that must be recalled.

**Q: Can I see the history of a specific bottle?**
Yes, the `trace_product_backward` tool allows you to reconstruct the entire history from a finished product back to its original grape lots.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-traceability-lot-tracking](https://vinkius.com/en/ai-agent-connect/wine-traceability-lot-tracking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Traceability & Lot Tracking** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-traceability-lot-tracking` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Traceability & Lot Tracking** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-traceability-lot-tracking": {
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
