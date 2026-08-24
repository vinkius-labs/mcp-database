# Quilting Block & Fabric Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/quilting-block-fabric-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate exact cutting dimensions, fabric yardage, and quilt layout for any block pattern.

## Description
This MCP server provides precise mathematical calculations for quilters. Use `calculate_block_pieces` to get exact cutting dimensions for patterns like half-square triangles or log cabins, accounting for seam allowances. Use `calculate_quilt_layout` to determine the total dimensions of your quilt including sashing and borders. Finally, use `calculate_fabric_requirements` to find the exact yardage needed for your fabric, batting, and backing, including whether your backing will need to be pieced.


## Available Tools (3)
- **calculate_block_pieces**: Determines the exact dimensions to cut for every individual fabric component required to assemble the specified block pattern
- **calculate_fabric_requirements**: Calculates the total yardage needed for each fabric color/position and the required dimensions for batting and backing
- **calculate_quilt_layout**: Calculates the total physical dimensions of the finished quilt based on block arrangement and decorative elements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Quilting Block & Fabric Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to make 10 half-square triangle blocks that are 5 inches finished. What do I need to cut?"

**🤖 AI Agent:**
> You will need to cut 10 background squares at 5.5 inches and 10 foreground triangles at 5.875 inches.

---

**👤 You:**
> "Calculate the total size of a quilt with 5 blocks wide, 6 blocks long, 2-inch sashing, and 3-inch borders."

**🤖 AI Agent:**
> The total quilt dimensions will be 37 inches wide by 44 inches long.

---

**👤 You:**
> "How much backing fabric do I need for a 60x70 inch quilt using 42-inch wide fabric?"

**🤖 AI Agent:**
> You will need 4.5 yards of backing, and since the width exceeds 42 inches, the backing will be pieced.


## ❓ FAQ

**Q: How does the tool handle seam allowances?**
The tool automatically adds a 1/2 inch seam allowance to standard pieces and a 7/8 inch allowance for half-square triangle components to ensure accuracy.

**Q: Can I calculate yardage for on-point quilt settings?**
Yes, by using `calculate_quilt_layout` with the `isOnPoint` parameter set to true, the tool calculates the correct dimensions and subsequent fabric needs.

**Q: What fabric width should I use?**
You can specify your fabric's usable width (typically 42 or 44 inches) in the `calculate_fabric_requirements` tool to get accurate yardage results.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/quilting-block-fabric-calculator](https://vinkius.com/ai-agent-connect/quilting-block-fabric-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Quilting Block & Fabric Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `quilting-block-fabric-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Quilting Block & Fabric Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "quilting-block-fabric-calculator": {
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
