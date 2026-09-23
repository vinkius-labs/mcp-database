# Room Light Count MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/room-light-count)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [architecture](../categories/architecture.md)

Calculate required light fixtures based on room area and lighting density.

## Description
This MCP server provides specialized tools for lighting design and planning. Use `get_fixture_count` to determine the exact number of lights needed for a space, `validate_lighting_density` to ensure coverage meets industry standards, and `compare_lighting_plans` to evaluate different lighting configurations. It also offers `get_standard_densities` to retrieve recommended coverage values for residential, commercial, or industrial environments.


## Available Tools (4)
- **compare_lighting_plans**: Each plan must be an object with roomArea and areaPerFixture.

Compares two different lighting configurations to see which one provides better coverage or more efficient fixture usage
- **get_fixture_count**: Calculates the total number of light fixtures needed for a specific room
- **get_standard_densities**: Retrieves a list of recommended area-per-fixture values based on the room category
- **validate_lighting_density**: Checks if a provided area per fixture value falls within industry-standard ranges for common room types


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Room Light Count** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many lights do I need for a 500 square foot room if each light covers 50 square feet?"

**🤖 AI Agent:**
> You will need 10 light fixtures for a 500 square foot room.

---

**👤 You:**
> "Is a density of 40 square meters per fixture appropriate for a residential room?"

**🤖 AI Agent:**
> The density of 40 square meters per fixture is within the recommended range for residential spaces.

---

**👤 You:**
> "Compare two plans: Plan A has 200sqft area and 20sqft per fixture. Plan B has 200sqft area and 25sqft per fixture."

**🤖 AI Agent:**
> Plan B is more efficient, requiring only 8 fixtures compared to Plan A's 10 fixtures.


## ❓ FAQ

**Q: How do I calculate the number of lights needed?**
You can use the `get_fixture_count` tool by providing the total room area and the area covered by a single fixture.

**Q: Can I use metric units?**
Yes, the `get_fixture_count` tool supports both imperial and metric unit systems.

**Q: How does the tool handle fractional results?**
The tool always rounds up to the nearest whole number to ensure full coverage of the specified area.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/room-light-count](https://vinkius.com/en/ai-agent-connect/room-light-count)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Room Light Count** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `room-light-count` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Room Light Count** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "room-light-count": {
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
