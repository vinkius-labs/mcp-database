# Seed Starting Tray Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/seed-starting-tray-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculates trays, cells, and labels needed for seed starting based on germination rates.

## Description
This MCP server helps growers plan their planting infrastructure. It calculates the exact number of physical trays, individual cells, and identification labels required to meet specific plant targets. By accounting for germination rates, it determines necessary backup cells to ensure your target plant count is met. Use `calculate_planting_requirements` to plan an entire session, `get_variety_summary` for specific variety details, `validate_tray_capacity` to check your inventory, or `generate_label_manifest` to prepare your labels.


## Available Tools (4)
- **calculate_planting_requirements**: Determines the total number of physical trays, individual cells, and necessary labels required for a specific list of plant varieties
- **generate_label_manifest**: Produces a list of all unique labels that need to be printed for a planting session
- **get_variety_summary**: Provides a focused breakdown of the infrastructure needed for a single specific plant variety
- **validate_tray_capacity**: Checks if a specific number of physical trays can accommodate a planned planting session


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Seed Starting Tray Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate requirements for 100 Tomato plants with 85% germination, 2 seeds per cell, using 72-cell trays."

**🤖 AI Agent:**
> To reach 100 Tomato plants with 85% germination, you need 118 total cells (118 cells including backup cells to account for the 15% failure rate). This requires 2 trays of 72-cell capacity.

---

**👤 You:**
> "I have 5 trays of 128-cell capacity. Can I plant 600 cells?"

**🤖 AI Agent:**
> Yes, your 5 trays provide a total capacity of 640 cells, which is sufficient to accommodate the 600 cells needed.

---

**👤 You:**
> "What are the specific requirements for 'Basil' in my list?"

**🤖 AI Agent:**
> For the Basil variety, you need 50 required cells and 10 backup cells, for a total of 60 seeds to plant.


## ❓ FAQ

**Q: How does the tool handle germination failure?**
The tool uses the provided germination rate to calculate 'backup cells'. These are extra cells planted to ensure you reach your target plant count even if some seeds fail to sprout.

**Q: Can I check if I have enough trays for my plan?**
Yes, you can use the `validate_tray_capacity` tool to compare your required cell count against your current tray inventory.

**Q: How do I get a list of labels to print?**
You can use the `generate_label_manifest` tool to produce a list of all unique variety names that require identification labels for your session.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/seed-starting-tray-calculator](https://vinkius.com/en/ai-agent-connect/seed-starting-tray-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Seed Starting Tray Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `seed-starting-tray-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Seed Starting Tray Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "seed-starting-tray-calculator": {
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
