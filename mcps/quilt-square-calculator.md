# Quilt Square Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/quilt-square-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Calculate precise square patch counts and material wastage for quilt making.

## Description
This MCP server provides precise mathematical tools for quilters to plan their projects. Use `get_square_distribution` to find how many full squares fit in a grid, `estimate_total_patches_needed` to determine the total number of patches to purchase, `check_fit_integrity` to see if a square size fits perfectly, or `calculate_material_wastage` to estimate leftover material. It bridges the gap between quilt dimensions and physical material requirements.


## Available Tools (4)
- **calculate_material_wastage**: Estimates the amount of material lost when cutting partial squares for the borders
- **check_fit_integrity**: Validates if a specific square size is mathematically "perfect" for a given quilt dimension (meaning no cutting is required)
- **estimate_total_patches_needed**: Determines the total number of individual patches (including partials) required to ensure full coverage of the quilt
- **get_square_distribution**: Calculates how many full squares fit in the grid and the specific dimensions of the remaining border


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Quilt Square Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a quilt that is 50x60 units. How many 5-unit squares will fit in a full grid?"

**🤖 AI Agent:**
> A 50x60 quilt with 5-unit squares will contain 120 full squares.

---

**👤 You:**
> "Will 10-unit squares fit perfectly in a 36x36 quilt?"

**🤖 AI Agent:**
> No, 10-unit squares will not fit perfectly. There will be a width gap of 6 units and a height gap of 6 units.

---

**👤 You:**
> "How many total patches do I need for a 36x36 quilt using 5-unit squares?"

**🤖 AI Agent:**
> You will need 64 total patches to ensure full coverage of the 36x36 quilt.


## ❓ FAQ

**Q: How do I know if my square size will fit perfectly?**
You can use the `check_fit_integrity` tool. It will tell you if the square size is a perfect fit or if there will be gaps at the edges.

**Q: How many patches should I buy for my quilt?**
Use the `estimate_total_patches_needed` tool. It calculates the total number of patches required to ensure full coverage, including partials.

**Q: Can I calculate how much fabric I will waste?**
Yes, the `calculate_material_wastage` tool provides the total wasted area and the usage efficiency of your patches.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/quilt-square-calculator](https://vinkius.com/en/ai-agent-connect/quilt-square-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Quilt Square Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `quilt-square-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Quilt Square Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "quilt-square-calculator": {
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
