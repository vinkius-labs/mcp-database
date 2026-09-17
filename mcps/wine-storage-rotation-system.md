# Wine Storage Rotation System MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-storage-rotation-system)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [inventory-management](../categories/inventory-management.md)

Manage wine inventory freshness using FIFO/FEFO rotation logic and aging models.

## Description
This MCP server provides advanced inventory management for wine cellars and warehouses. It uses aging models, vintage data, and sales velocity to manage stock risk and rotation schedules. Use `get_rotation_schedule` to identify which bottles to move first, `check_oldest_stock_alerts` to find aged batches, `calculate_overaging_risk` to assess quality loss based on wine style and closure type, and `analyze_inventory_health` for a complete overview of storage efficiency.


## Available Tools (4)
- **get_rotation_schedule**: Which bottles should I move or sell first to maintain optimal inventory freshness?
- **analyze_inventory_health**: What is the overall status of our aging profile and storage efficiency?
- **calculate_overaging_risk**: How much stock is at risk of losing quality before we can sell it?
- **check_oldest_stock_alerts**: Which specific vintages or batches are currently the oldest in our warehouse?


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Storage Rotation System** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which bottles should I move or sell first to maintain optimal inventory freshness?"

**🤖 AI Agent:**
> You should prioritize moving the 2018 Cabernet Sauvignon and the 2019 Chardonnay to maintain freshness.

---

**👤 You:**
> "Which specific vintages or batches are currently the oldest in our warehouse?"

**🤖 AI Agent:**
> The oldest items currently flagged are the 2012 Merlot and the 2010 Bordeaux.

---

**👤 You:**
> "How much stock is at risk of losing quality before we can sell it for a heavy red with a cork seal?"

**🤖 AI Agent:**
> The risk level is medium, with an estimated 45 days remaining until the peak window ends.


## ❓ FAQ

**Q: How does the rotation logic work?**
The system uses FEFO (First-Expired, First-Out) logic to prioritize stock approaching the end of its peak drinking window, ensuring optimal freshness.

**Q: Can I check for specific aged batches?**
Yes, you can use the `check_oldest_stock_alerts` tool to identify specific vintages or batches that have exceeded your defined age threshold.

**Q: How is over-aging risk calculated?**
Risk is calculated by comparing the predicted peak drinking window (determined by wine style and closure type) against current sales velocity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-storage-rotation-system](https://vinkius.com/en/ai-agent-connect/wine-storage-rotation-system)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Storage Rotation System** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-storage-rotation-system` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Storage Rotation System** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-storage-rotation-system": {
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
