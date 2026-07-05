# Accessibility Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/accessibility-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Verify building compliance against universal accessibility standards (USA/EU) for corridors, ramps, and restrooms.

## Description
**Goal:** Ensure every physical space meets minimum dimensions required for people with reduced mobility.

**Problem:** Building designs often fail to meet modern accessibility standards (like ADA or European norms). A small mistake in a corridor width, ramp slope, or bathroom layout can render an entire facility unusable and dangerous. Failing compliance blocks safe passage for wheelchairs and other aids.

**Mechanism:** This service provides precise checks across all critical architectural elements using specialized tools:
*   `check_corridor_and_passage`: Verifies that hallways maintain a minimum clear width throughout their length.
*   `check_ramp_compliance`: Calculates the slope of ramps and confirms adequate resting landings at every transition point.
*   `check_doorway`: Measures the actual clear opening width to ensure passage is possible for mobility aids.
*   `check_bathroom_spaciousness`: Confirms that restrooms provide enough functional floor area and maneuvering space, going beyond simple dimensions.

**Advantage:** By running these checks, you receive an immediate compliance report detailing every violation--from minor dimension gaps to critical structural failures--allowing architects and builders to correct issues before construction begins.


## Available Tools (4)
- **check_corridor_and_passage**: Returns compliance status and violation details.

Verify corridor or passage meets minimum clear width for universal access
- **check_doorway**: Verify doorway provides adequate clear opening width for mobility aid users
- **check_ramp_compliance**: 33% maximum standard and checks for required transition landings.

Determine if a ramp section meets maximum slope and landing requirements
- **check_bathroom_spaciousness**: Confirm bathroom provides enough functional space for mobility aid maneuverability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessibility Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze Room 302. The corridor ID is 'P-MAIN', the measured width is 1.05m, and I need to check ramp compliance for a drop of 1.8m over a horizontal run of 15m with landings."

**🤖 AI Agent:**
> Running checks: `check_corridor_and_passage` confirms passage 'P-MAIN' is compliant (1.05m). `check_ramp_compliance` determines the slope and verifies landing requirements are met.

---

**👤 You:**
> "I need to check a restroom, Room ID 'B-401'. The usable floor area is 2.5 sq meters, and I have installed grab bars."

**🤖 AI Agent:**
> Using `check_bathroom_spaciousness` on Room 'B-401', the tool confirms the area is adequate (2.5m²), and verifies that safety grab bars are in place, ensuring functional compliance.

---

**👤 You:**
> "Check a doorway at 'Lecture Hall Entrance'. The clear opening is 0.9m, and it's a sliding door."

**🤖 AI Agent:**
> The `check_doorway` tool analyzed the location. With an unobstructed width of 0.9m for the 'Lecture Hall Entrance', compliance is confirmed, meeting minimum accessibility standards.


## ❓ FAQ

**Q: What is the minimum width required for a main corridor?**
The system uses the `check_corridor_and_passage` tool to verify this. It checks the measured clear width against mandatory standards, ensuring safe passage for mobility aids.

**Q: Does it check if ramps are steep enough?**
The `check_ramp_compliance` tool handles slope and landings. It calculates the ratio to ensure it does not exceed the maximum permitted standard (e.g., 8.33%) and verifies landing presence.

**Q: Are doorways checked for proper clearance?**
Yes, the `check_doorway` tool specifically measures the unobstructed clear opening width. This guarantees that passage is possible regardless of the door's hardware or type.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/accessibility-checker](https://vinkius.com/mcp/accessibility-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessibility Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessibility-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessibility Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessibility-checker": {
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
