# Door Clearance Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/door-clearance-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Verify if furniture can fit through specific doorways.

## Description
This MCP server provides tools to determine if furniture can physically pass through architectural openings. Use `get_door_clearance` to find the usable width of a doorway, `check_furniture_fit` to compare furniture dimensions against door clearance with an optional safety buffer, `list_furniture_by_category` to browse inventory, and `validate_dimensions` to ensure measurements are realistic.


## Available Tools (4)
- **check_furniture_fit**: Determines if a specific piece of furniture can pass through a specified doorway
- **get_door_clearance**: Retrieves the usable width of a specific doorway
- **list_furniture_by_category**: Retrieves a list of furniture items filtered by their type
- **validate_dimensions**: Ensures that all provided measurements for an object or opening are physically possible


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Door Clearance Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Will the sofa with ID 'sofa-123' fit through door 'door-456'?"

**🤖 AI Agent:**
> Yes, the sofa will fit through the door with a remaining margin of 5cm.

---

**👤 You:**
> "What is the usable width of door 'main-entrance'?"

**🤖 AI Agent:**
> The usable width for the main entrance is 90cm.

---

**👤 You:**
> "List all chairs available in the catalog."

**🤖 AI Agent:**
> The available chairs are: Dining Chair (ID: chair-01), Office Chair (ID: chair-02), and Lounge Chair (ID: chair-03).


## ❓ FAQ

**Q: How does the tool calculate if a piece of furniture fits?**
The tool uses `check_furniture_fit` to compare the smallest dimension of the furniture against the usable width provided by `get_door_clearance`, optionally subtracting a safety buffer.

**Q: Can I include a safety margin in the calculation?**
Yes, when using `check_furniture_fit`, you can provide a `safetyBuffer` value to ensure a comfortable fit.

**Q: What happens if the door ID is incorrect?**
If an invalid `doorId` is provided to `get_door_clearance` or `check_furniture_fit`, the tool will return an error.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/door-clearance-checker](https://vinkius.com/en/ai-agent-connect/door-clearance-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Door Clearance Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `door-clearance-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Door Clearance Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "door-clearance-checker": {
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
