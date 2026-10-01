# Clay Reclaim Yield Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/clay-reclaim-yield-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [manufacturing](../categories/manufacturing.md)

Calculate usable reclaimed clay from scrap weight, moisture loss, and contamination.

## Description
This MCP server provides precision calculation tools for managing the circular economy of clay in ceramic production. It allows AI agents to determine the exact amount of usable material extracted from scrap, calculate necessary fresh clay additions to meet production targets, and analyze batch compositions. Use `get_reclaimed_yield` to find usable mass, `calculate_required_fresh_clay` to plan additions, `estimate_batch_composition` for material ratios, and `validate_production_feasibility` to check if existing scrap meets your needs.


## Available Tools (4)
- **validate_production_feasibility**: Check if a specific scrap supply is sufficient to meet a target without needing any fresh clay additions
- **calculate_required_fresh_clay**: Determine how much new clay must be added to the reclaimed material to meet a production goal
- **estimate_batch_composition**: Provide a full breakdown of a target batch, showing the ratio of recycled material to fresh material
- **get_reclaimed_yield**: Determine how much usable clay can be extracted from a specific amount of scrap


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clay Reclaim Yield Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much usable clay can I get from 500kg of scrap with 5% moisture loss and 2% contamination?"

**🤖 AI Agent:**
> You can extract 465kg of usable reclaimed clay.

---

**👤 You:**
> "I have 400kg of reclaimed clay. How much fresh clay do I need to reach a 500kg batch?"

**🤖 AI Agent:**
> You need to add 100kg of fresh clay to reach the 500kg target.

---

**👤 You:**
> "Is 300kg of scrap enough for a 250kg batch if there is 10% moisture loss and 5% contamination?"

**🤖 AI Agent:**
> Yes, the reclaimed yield is 255kg, which is sufficient for the 250kg target.


## ❓ FAQ

**Q: How does the tool account for material loss?**
The `get_reclaimed_yield` tool subtracts both the weight lost to moisture evaporation and the weight lost to contamination from the original scrap weight.

**Q: Can I check if my current scrap is enough for a batch?**
Yes, you can use `validate_production_feasibility` to determine if your available scrap meets the target batch size without needing fresh clay.

**Q: What information is needed to calculate fresh clay requirements?**
To use `calculate_required_fresh_clay`, you need the weight of the usable reclaimed yield and the desired total target batch size.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/clay-reclaim-yield-estimator](https://vinkius.com/en/ai-agent-connect/clay-reclaim-yield-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Clay Reclaim Yield Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `clay-reclaim-yield-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Clay Reclaim Yield Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clay-reclaim-yield-estimator": {
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
