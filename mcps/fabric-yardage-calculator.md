# Fabric Yardage Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fabric-yardage-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate precise fabric requirements for custom patterns, garments, and projects.

## Description
The Fabric Yardage Calculator MCP connects your AI agent to a specialized engine for estimating textile needs. Use `calculate_custom_layout` to determine the linear length required for specific pattern pieces, accounting for nap direction and pattern repeats. The `lookup_garment_yardage` tool provides quick estimates for standard clothing sizes from XS to 5XL. For larger textile projects, `calculate_project_fabric` calculates the necessary yardage for curtains (including fullness) and quilts. This server ensures accuracy by supporting various fabric widths including 45\", 5/4\", 60\", 110cm, and 150cm.


## Available Tools (3)
- **calculate_custom_layout**: Supports one-way or two-way nap direction.

Calculates the total linear fabric length required for a custom set of pattern pieces
- **calculate_project_fabric**: Calculates fabric requirements for non-garment projects like curtains or quilts
- **lookup_garment_yardage**: Retrieves estimated yardage from the database for standard clothing items


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fabric Yardage Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much fabric do I need for a T-shirt in size Large using 60 inch fabric?"

**🤖 AI Agent:**
> For a size L T-Shirt on 60\" fabric, you will need approximately 0.75 yards (0.68 meters).

---

**👤 You:**
> "Calculate the yardage for a custom layout with two pieces: one 10x20 inches and one 15x30 inches, using 45 inch fabric and one-way nap."

**🤖 AI Agent:**
> The total length required is 0.83 yards (0.76 meters) with an efficiency score of 75%.

---

**👤 You:**
> "How much fabric is needed for a curtain that is 50 inches wide and 80 inches long, assuming 2.0 fullness?"

**🤖 AI Agent:**
> You will need 4.44 yards (4.06 meters) of fabric, which will require 2 panels.


## ❓ FAQ

**Q: How do I calculate fabric for a custom pattern piece?**
Use the `calculate_custom_layout` tool. Provide the widths and lengths of your pieces, the fabric width, and whether you are using a one-way or two-way nap direction.

**Q: Can I account for stripes or plaids?**
Yes. When using `calculate_custom_layout`, you can provide a `patternRepeatLength`. The tool will automatically add one full repeat to the total length to ensure proper alignment.

**Q: What garment sizes are supported?**
The `lookup_garment_yardage` tool supports standard sizing from XS up to 5XL.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fabric-yardage-calculator](https://vinkius.com/mcp/fabric-yardage-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fabric Yardage Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fabric-yardage-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fabric Yardage Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fabric-yardage-calculator": {
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
