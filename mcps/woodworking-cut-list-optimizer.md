# Woodworking Cut List Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/woodworking-cut-list-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [optimization](../categories/optimization.md)

Minimize lumber waste with deterministic 1D bin packing for cutting plans.

## Description
This MCP server provides precise tools for woodworking professionals to minimize material waste. By applying deterministic 1D bin packing algorithms, it calculates the most efficient way to cut required pieces from available lumber stock. Use `cut_list_optimizer` to generate complete cutting diagrams, `validate_cut_plan` to verify specific sequences, and `calculate_material_efficiency` to track your material yield. It accounts for saw kerf width to ensure every cut is physically possible and accurate.


## Available Tools (3)
- **calculate_material_efficiency**: Compares the total useful wood against the total wood consumed to determine yield
- **cut_list_optimizer**: Generates an optimized cutting plan to minimize waste using available lumber
- **validate_cut_plan**: Verifies if a specific proposed cutting sequence is physically possible given the constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Woodworking Cut List Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate an optimized cutting plan for 3 pieces of 500mm and 2 pieces of 800mm using two 2400mm boards with a 3mm kerf."

**🤖 AI Agent:**
> Board 1: Cut 800mm, 800mm, 500mm. Waste: 297mm. Board 2: Cut 500mm, 500mm, 500mm. Waste: 897mm. Total Yield: 75.4%.

---

**👤 You:**
> "Is it possible to cut three 700mm pieces from a 2000mm board with a 5mm kerf?"

**🤖 AI Agent:**
> No, the total length required for three 700mm pieces and two 5mm kerfs is 2110mm, which exceeds the 2000mm board length.

---

**👤 You:**
> "Calculate the efficiency if I used 1500mm of wood out of 2000mm total."

**🤖 AI Agent:**
> The material yield is 75% and the waste is 25%.


## ❓ FAQ

**Q: How does the optimizer handle saw kerf?**
The `cut_list_optimizer` tool automatically includes the specified `kerfWidth` between every piece cut, ensuring the total length used never exceeds the actual board length.

**Q: Can I verify a manual cutting plan?**
Yes, you can use the `validate_cut_plan` tool to check if a specific sequence of cuts is physically possible given your board length and saw kerf.

**Q: What is material yield?**
Material yield is the percentage of total available wood that becomes usable pieces. You can calculate this using `calculate_material_efficiency`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/woodworking-cut-list-optimizer](https://vinkius.com/ai-agent-connect/woodworking-cut-list-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Woodworking Cut List Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `woodworking-cut-list-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Woodworking Cut List Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "woodworking-cut-list-optimizer": {
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
