# Button Sizing Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/button-sizing-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Converts button sizes between Ligne, mm, and inches, and calculates buttonhole dimensions.

## Description
The Button Sizing Engine is a specialized utility for the garment manufacturing industry. It provides precise conversions between Ligne (L), millimeters (mm), and inches (in) for button diameters using `convert_button_unit`. The engine includes tools like `get_button_by_application` to find standard sizes for specific garment parts like shirt cuffs or coat closures, `calculate_buttonhole_dimensions` to determine the necessary hole length including a thread margin, and `estimate_button_spacing` to suggest optimal button placement based on fabric weight.


## Available Tools (4)
- **get_button_by_application**: Gets standard button size for a garment part
- **calculate_buttonhole_dimensions**: Calculates necessary buttonhole length
- **convert_button_unit**: Converts a dimension from one unit to another
- **estimate_button_spacing**: Suggests ideal distance between buttons


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Button Sizing Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert 20L to millimeters."

**🤖 AI Agent:**
> 20L is equal to 5.08 mm.

---

**👤 You:**
> "What button size should I use for a shirt cuff?"

**🤖 AI Agent:**
> For a shirt cuff, the recommended size is 16L (approximately 4.06 mm).

---

**👤 You:**
> "Calculate the buttonhole length for a 12mm button."

**🤖 AI Agent:**
> The minimum required buttonhole length is 15 mm.


## ❓ FAQ

**Q: How accurate are the unit conversions?**
The `convert_button_unit` tool uses standardized industry ratios to ensure high precision between Ligne, mm, and inches.

**Q: How is the buttonhole length calculated?**
The `calculate_buttonhole_dimensions` tool takes the button diameter in mm and adds a 3mm margin to account for thread thickness and fabric bulk.

**Q: Can I find recommended sizes for specific clothing parts?**
Yes, using `get_button_by_application`, you can retrieve standard Ligne sizes and diameters for items like shirt cuffs or coat closures.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/button-sizing-engine](https://vinkius.com/mcp/button-sizing-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Button Sizing Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `button-sizing-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Button Sizing Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "button-sizing-engine": {
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
