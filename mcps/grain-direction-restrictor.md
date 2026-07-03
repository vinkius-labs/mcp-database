# Grain Direction Restrictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/grain-direction-restrictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [optimization](../categories/optimization.md)

Enforce material grain orientation constraints for precise plywood cutting and bin packing.

## Description
The Grain Direction Restrictor is a specialized constraint engine designed for wood and plywood processing. It prevents illegal rotations of material pieces during the cutting process by enforcing intrinsic grain directions (horizontal or vertical). By using tools like `validate_single_piece`, `get_oriented_dimensions`, and `evaluate_batch_constraints`, you can ensure that every piece in your batch maintains its structural integrity relative to the stock sheet dimensions. This is critical for preventing waste-inducing errors in complex bin packing algorithms where rotation is restricted by material properties.


## Available Tools (3)
- **evaluate_batch_constraints**: Scans a batch of pieces for maximum required dimensions and invalidity
- **get_oriented_dimensions**: Calculates the effective footprint of a piece based on grain orientation
- **validate_single_piece**: Verifies if a single piece fits within stock dimensions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Grain Direction Restrictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if a 50x100 piece with vertical grain fits in a 120x240 sheet."

**🤖 AI Agent:**
> Yes, the piece is compatible. The effective footprint for vertical orientation is 100x50, which fits within the 120x240 stock dimensions.

---

**👤 You:**
> "Calculate the effective width and length for a 30cm x 60cm piece with horizontal grain."

**🤖 AI Agent:**
> The effective width is 30cm and the effective length is 60cm.

---

**👤 You:**
> "Will a 250x150 piece with horizontal grain fit in a 240x120 sheet?"

**🤖 AI Agent:**
> No, the piece exceeds the stock dimensions. The required width of 250cm is greater than the available stock width of 240cm.


## ❓ FAQ

**Q: How does the tool handle vertical grain orientation?**
When `grainDirection` is set to 'vertical', the tool swaps the piece's width and length mapping. The intrinsic width is checked against the stock length, and the intrinsic length is checked against the stock width.

**Q: Can I use this for standard bin packing without grain constraints?**
While you can set all pieces to a single orientation, this tool is specifically built to enforce the restriction that prevents rotation. If you need free rotation, you would typically use a different optimization engine.

**Q: What happens if a piece exceeds the stock dimensions?**
The `validate_single_piece` tool will return a failure status with an error message indicating whether the oriented width or length exceeded the available stock limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/grain-direction-restrictor](https://vinkius.com/mcp/grain-direction-restrictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Grain Direction Restrictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `grain-direction-restrictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Grain Direction Restrictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "grain-direction-restrictor": {
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
