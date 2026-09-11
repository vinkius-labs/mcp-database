# Completion Accessories Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/completion-accessories-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design downhole completion accessories by analyzing well conditions and operational requirements.

## Description
This MCP server provides specialized engineering tools for designing downhole completion accessories. It allows users to determine appropriate nipple profiles using `get_nipple_specifications`, calculate optimal vertical positions with `calculate_landing_depths`, define flow control characteristics via `determine_sleeve_requirements`, and verify maintenance feasibility through `validate_intervention_access`. It bridges the gap between wellbore architecture and physical equipment placement.


## Available Tools (4)
- **calculate_landing_depths**: Calculates the optimal vertical depths for placing landing nipples
- **determine_sleeve_requirements**: Defines the necessary characteristics and placements for sliding sleeves
- **get_nipple_specifications**: Determines the appropriate nipple profiles required for a specific completion design
- **validate_intervention_access**: Verifies if the designed accessory string allows for intended future maintenance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Completion Accessories Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What nipple profiles do I need for a cased-perforated well with high pressure?"

**🤖 AI Agent:**
> For a cased-perforated well under high pressure, the recommended profiles are Medium and Heavy profiles to ensure mechanical integrity.

---

**👤 You:**
> "Calculate the landing depths for nipples at 5000m and 7500m with a 50m clearance."

**🤖 AI Agent:**
> The calculated nipple depths are 4950m and 7450m to maintain the required 50m safety margin.

---

**👤 You:**
> "Will a 2.5 inch tool fit in a completion with a 3.0 inch internal diameter?"

**🤖 AI Agent:**
> Yes, the tool is compatible with the completion internal diameter.


## ❓ FAQ

**Q: How do I determine which nipple profiles are suitable?**
You can use the `get_nipple_specifications` tool by providing the completion type and the specific well conditions like pressure and temperature.

**Q: Can I check if my wireline tools will fit in the design?**
Yes, use the `validate_intervention_access` tool to verify if the tool diameter is compatible with the completion internal diameter and nipple locations.

**Q: How are sliding sleeve depths determined?**
The `determine_sleeve_requirements` tool calculates the necessary sleeve types and depths based on target depths, wireline compatibility, and operational pressure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/completion-accessories-design](https://vinkius.com/en/ai-agent-connect/completion-accessories-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Completion Accessories Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `completion-accessories-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Completion Accessories Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "completion-accessories-design": {
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
