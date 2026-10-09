# Sewing Fabric Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sewing-fabric-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate the exact fabric length needed for your sewing projects.

## Description
This MCP server provides essential tools for sewing and textile planning. It helps you determine the linear length of fabric required by analyzing pattern piece areas, fabric width, and waste buffers. You can use `get_fabric_requirement` to find the total length, `validate_fabric_width` to check if your fabric is standard, `get_pattern_summary` for a material overview, and `estimate_waste_buffer` to suggest extra fabric for complex shapes.


## Available Tools (4)
- **estimate_waste_buffer**: Suggests an appropriate waste percentage based on the complexity of the pattern pieces
- **get_fabric_requirement**: Calculates the total linear length of fabric needed for a specific set of pattern pieces
- **get_pattern_summary**: Provides a high-level overview of the total material needs before calculating length
- **validate_fabric_width**: Checks if a provided fabric width is standard and usable for sewing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sewing Fabric Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have three pattern pieces with areas of 50, 30, and 20 square inches. My fabric is 45 inches wide. What is the total length I need with a 15% waste buffer?"

**🤖 AI Agent:**
> You will need 2.30 inches of fabric.

---

**👤 You:**
> "What is the total area of my pattern pieces if they are 120, 85, and 45 square units?"

**🤖 AI Agent:**
> The total area of your pattern pieces is 250 square units.

---

**👤 You:**
> "Is a fabric width of 30 inches standard for sewing?"

**🤖 AI Agent:**
> Yes, a 30-inch fabric width is considered a standard and usable width for sewing.


## ❓ FAQ

**Q: How do I know how much fabric to buy?**
You can use the `get_fabric_requirement` tool. Provide the areas of your pattern pieces, the width of your fabric, and your preferred waste percentage to get the total linear length needed.

**Q: What is a waste percentage?**
A waste percentage is a buffer added to your calculation to account for fabric lost during cutting and the gaps between irregular pattern pieces. You can use `estimate_waste_buffer` to help decide this value.

**Q: Can I check if my fabric width is standard?**
Yes, the `validate_fabric_width` tool checks if your provided width falls within common industry standards for sewing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sewing-fabric-calculator](https://vinkius.com/en/ai-agent-connect/sewing-fabric-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sewing Fabric Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sewing-fabric-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sewing Fabric Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sewing-fabric-calculator": {
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
