# Wardrobe Donation Weight Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wardrobe-donation-weight-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [charity](../categories/charity.md)

Track garment weights and manage donation batch logistics.

## Description
This MCP server provides tools for charitable organizations to manage clothing donation logistics. It allows users to record individual items using `add_garment`, monitor if a collection is ready for transport with `calculate_batch_status`, view detailed composition via `get_batch_summary`, and manage multiple collections with `list_batches`.


## Available Tools (4)
- **calculate_batch_status**: Determines the logistics readiness of a donation batch
- **get_batch_summary**: Provides a high-level overview of a batch's composition
- **list_batches**: Retrieves a list of all active donation batches
- **add_garment**: Adds a single piece of clothing to a specific donation batch


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wardrobe Donation Weight Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Add a 2kg blue shirt to batch B123."

**🤖 AI Agent:**
> The shirt has been added. The current batch weight is 2kg and there is 1 item in the batch.

---

**👤 You:**
> "Is batch B123 ready for pickup if the target is 10kg?"

**🤖 AI Agent:**
> No, the batch is not ready. There is 8kg of capacity remaining before the target is reached.

---

**👤 You:**
> "Show me all batches that weigh more than 50kg."

**🤖 AI Agent:**
> Found 1 batch: Batch ID 'BULK-001' with a total weight of 55kg.


## ❓ FAQ

**Q: How do I add a new item to a donation batch?**
Use the `add_garment` tool by providing the batch ID, the weight of the item, and the type of garment.

**Q: How can I tell if a batch is ready to be picked up?**
You can use `calculate_batch_status` with a target capacity to see if the batch has reached the weight required for pickup.

**Q: Can I see a breakdown of what is in a batch?**
Yes, the `get_batch_summary` tool provides the total weight, item count, and a distribution of garment types.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wardrobe-donation-weight-tracker](https://vinkius.com/en/ai-agent-connect/wardrobe-donation-weight-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wardrobe Donation Weight Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wardrobe-donation-weight-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wardrobe Donation Weight Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wardrobe-donation-weight-tracker": {
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
