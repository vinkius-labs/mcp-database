# Darkroom Chemical Mixing Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/darkroom-chemical-mixing-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate precise water and concentrate volumes for darkroom chemical solutions.

## Description
This MCP server provides precision calculation tools for darkroom technicians. It automates the math required to prepare working solutions by determining exact water and concentrate volumes based on dilution ratios, tray counts, and waste margins. Use `generate_full_mixing_plan` to create a complete session plan or `calculate_single_mix_batch` for individual chemical needs.


## Available Tools (4)
- **calculate_tray_requirements**: Determines the minimum total volume required based on the physical setup of the darkroom
- **generate_full_mixing_plan**: A high-level orchestrator that calculates all necessary components for a complete darkroom session
- **validate_chemical_stock**: Checks if a requested chemical is available in the predefined chemical catalog
- **calculate_single_mix_batch**: Calculates the specific volumes of concentrate and water needed for one specific chemical type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Darkroom Chemical Mixing Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to fill 3 trays with 500ml each, with a 10% waste margin. I need Developer (1:10) and Stop Bath (1:5)."

**🤖 AI Agent:**
> For 3 trays at 500ml each with 10% waste, the total session volume is 1650ml. Your plan is: Developer: 165ml concentrate and 1485ml water; Stop Bath: 330ml concentrate and 1320ml water.

---

**👤 You:**
> "How much water and concentrate do I need for 1 liter of a 1:9 Developer solution?"

**🤖 AI Agent:**
> For 1 liter of a 1:9 Developer solution, you need 100ml of concentrate and 900ml of water.

---

**👤 You:**
> "Check if 'Fixer' is a valid chemical in the catalog."

**🤖 AI Agent:**
> Yes, 'Fixer' is a valid chemical in the authorized catalog.


## ❓ FAQ

**Q: How do I calculate the total volume needed for my session?**
You can use the `calculate_tray_requirements` tool to determine the total volume based on your tray count and the volume required per tray, including a safety waste margin.

**Q: Can I plan a whole session at once?**
Yes, the `generate_full_mixing_plan` tool allows you to input your tray requirements and a list of chemical requests to get a complete mixing plan for the entire session.

**Q: How does the waste allowance work?**
The waste allowance is a percentage added to your total volume to account for spills or residue, ensuring you have enough solution to complete your work.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/darkroom-chemical-mixing-plan](https://vinkius.com/en/ai-agent-connect/darkroom-chemical-mixing-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Darkroom Chemical Mixing Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `darkroom-chemical-mixing-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Darkroom Chemical Mixing Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "darkroom-chemical-mixing-plan": {
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
