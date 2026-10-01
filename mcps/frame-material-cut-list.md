# Frame Material Cut List MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/frame-material-cut-list)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [optimization](../categories/optimization.md)

Calculates optimal cutting patterns, stock usage, and offcuts for picture frame manufacturing.

## Description
This MCP server provides precision tools for picture frame production. It calculates exact piece lengths using miter geometry and optimizes material usage by nesting required pieces into available stock lengths. Use `calculate_cut_list` to generate a full production schedule, `validate_material_feasibility` to check if dimensions fit your stock, or `compare_stock_efficiency` to minimize waste between different stock options.


## Available Tools (4)
- **calculate_cut_list**: Generates the complete cutting schedule including pieces, used stock, and offcuts
- **compare_stock_efficiency**: Evaluates which of two different stock lengths would result in less total waste for a specific order
- **get_piece_dimensions**: Calculates the exact cut length for a single piece based on frame geometry
- **validate_material_feasibility**: Checks if a specific set of artwork dimensions can physically be cut from the available stock


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Frame Material Cut List** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a cut list for 5 frames. Artwork is 10x12, frame width is 2, miter allowance is 0.5, and stock length is 96."

**🤖 AI Agent:**
> To produce 5 frames, you need 10 pieces of 15.0 units and 10 pieces of 17.0 units. This requires 4 stock pieces of 96 units, with a total of 5 offcuts.

---

**👤 You:**
> "Is it possible to make a frame for a 20x20 artwork with a 3-inch frame and 0.25 miter allowance using 48-inch stock?"

**🤖 AI Agent:**
> No, the required piece length is 26.5 inches, and while a single piece fits, the total material required for all four sides exceeds the capacity of a single 48-inch stock piece.

---

**👤 You:**
> "Which is better for 10 frames (12x12, 1.5 width, 0.2 allowance): 96-inch stock or 120-inch stock?"

**🤖 AI Agent:**
> The 120-inch stock length is more efficient, reducing total waste by 14.5 units compared to the 96-inch option.


## ❓ FAQ

**Q: How does the tool calculate piece lengths?**
The length is calculated by adding the artwork dimension, twice the frame width, and twice the miter allowance.

**Q: Can I compare different stock lengths?**
Yes, you can use `compare_stock_efficiency` to determine which stock length results in the least amount of total waste.

**Q: What happens if a piece is too long for my stock?**
If a piece exceeds the provided stock length, `validate_material_feasibility` will return a failure reason explaining the constraint.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/frame-material-cut-list](https://vinkius.com/en/ai-agent-connect/frame-material-cut-list)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Frame Material Cut List** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `frame-material-cut-list` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Frame Material Cut List** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "frame-material-cut-list": {
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
