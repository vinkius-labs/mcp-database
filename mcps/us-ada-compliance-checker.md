# US ADA Compliance Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-ada-compliance-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Verify architectural elements against US ADA accessibility standards.

## Description
The US ADA Compliance Checker provides automated verification for critical architectural dimensions to ensure compliance with the Americans with Disabilities Act (ADA). Use tools like `check_ramp_compliance` to validate ramp slopes, `check_door_clearance_compliance` for doorway widths, and `check_parking_access_compliance` for parking stall and aisle requirements. It also covers `check_restroom_maneuverability_compliance` for turning diameters and `check_corridor_width_compliance` for hallway clearances.


## Available Tools (5)
- **check_corridor_width_compliance**: Ensures corridors provide enough width for passage and passing
- **check_door_clearance_compliance**: Verifies if a doorway provides enough width for unobstructed passage
- **check_parking_access_compliance**: Validates that both the parking stall and the access aisle meet accessibility dimensions
- **check_ramp_compliance**: Determines if a ramp's incline meets the maximum allowed steepness
- **check_restroom_maneuverability_compliance**: Checks if there is enough diameter within a restroom to allow for a wheelchair turn


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US ADA Compliance Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is a ramp with a 2-inch rise and 30-inch run compliant?"

**🤖 AI Agent:**
> No, the slope is 1:15, which exceeds the maximum allowed ratio of 1:12.

---

**👤 You:**
> "Check if a 36-inch door is wide enough."

**🤖 AI Agent:**
> Yes, a 36-inch width meets the minimum requirement of 32 inches.

---

**👤 You:**
> "Is a 65-inch turning diameter sufficient for a restroom?"

**🤖 AI Agent:**
> Yes, the 65-inch diameter exceeds the minimum requirement of 60 inches.


## ❓ FAQ

**Q: How do I check if a ramp is compliant?**
Use the `check_ramp_compliance` tool by providing the vertical rise and horizontal run. The tool will check if the slope is within the 1:12 maximum ratio.

**Q: What is the minimum width for a doorway?**
The clear width of a doorway must be at least 32 inches. You can verify this using the `check_door_clearance_compliance` tool.

**Q: Can I check parking stall requirements?**
Yes, use `check_parking_access_compliance` and provide the stall width (min 8') and aisle width (min 5').


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-ada-compliance-checker](https://vinkius.com/mcp/us-ada-compliance-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US ADA Compliance Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-ada-compliance-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US ADA Compliance Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-ada-compliance-checker": {
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
