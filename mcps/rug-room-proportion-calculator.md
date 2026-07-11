# Rug & Room Proportion Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rug-room-proportion-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [interior-design](../categories/interior-design.md)

Validate if rug dimensions follow professional interior design rules for floor borders and furniture anchoring.

## Description
Ensure your space looks professionally designed by verifying that your rug placement adheres to spatial standards. This MCP server provides tools like `verify_floor_border` to check for the essential 12-inch bare floor perimeter and `verify_furniture_anchoring` to confirm if your rug properly supports furniture layouts such as 'all_on_rug' or 'front_legs_on'. Use `get_design_compliance_report` for a complete audit of your room's proportions.


## Available Tools (3)
- **verify_furniture_anchoring**: Validates rug adequacy based on furniture layout
- **verify_floor_border**: Returns compliance status and dimensions.

Checks if the rug leaves a sufficient 12-inch bare floor border
- **get_design_compliance_report**: Aggregates all spatial checks into a single pass/fail audit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rug & Room Proportion Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is my rug placement correct? Room: 144x144 inches, Rug: 108x108 inches, Layout: all_on_rug."

**🤖 AI Agent:**
> The rug placement is compliant. The floor border is 18 inches on all sides, satisfying the 12-inch minimum requirement.

---

**👤 You:**
> "Check if this rug works for a 'front_legs_on' layout. Rug length: 96 inches, Sofa depth: 36 inches."

**🤖 AI Agent:**
> The rug is appropriately anchored. The required length for the sofa depth is 78 inches (36 + 2 * 21), and your 96-inch rug exceeds this.

---

**👤 You:**
> "Will a 60x60 inch rug work in a 70x70 inch room with a 'floating' layout?"

**🤖 AI Agent:**
> The rug fails the border rule. The margin is only 5 inches, which is less than the required 12-inch bare floor border.


## ❓ FAQ

**Q: How does the floor border check work?**
The `verify_floor_border` tool calculates the margin between the rug edges and the room walls. It returns a pass if there is at least a 12-inch gap on all sides.

**Q: What layouts can I validate?**
You can validate three primary strategies: 'all_on_rug', 'front_legs_on', and 'floating' using the `verify_furniture_anchoring` tool.

**Q: Can I get a full report of all design rules?**
Yes, the `get_design_compliance_report` tool aggregates both border and anchoring checks into a single pass/fail audit.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rug-room-proportion-calculator](https://vinkius.com/mcp/rug-room-proportion-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rug & Room Proportion Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rug-room-proportion-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rug & Room Proportion Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rug-room-proportion-calculator": {
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
