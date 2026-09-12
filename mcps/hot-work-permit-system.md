# Hot Work Permit System MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/hot-work-permit-system)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [compliance](../categories/compliance.md)

Automated safety compliance for hot work operations.

## Description
This MCP server provides specialized safety management for hot work operations like welding, cutting, and grinding. It calculates regulatory compliance requirements based on NFPA 51B and API standards, including fire watch durations, exclusion zone radii, and atmospheric monitoring needs.


## Available Tools (4)
- **calculate_exclusion_zone**: Defines the physical radius of the safety perimeter around the hot work
- **calculate_fire_watch**: Determines if a fire watch is required and how long they must remain on-site
- **check_atmospheric_safety**: Evaluates if the air quality must be monitored before and during work
- **generate_permit_summary**: Aggregates all safety requirements into a single summary for a work permit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hot Work Permit System** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is a fire watch required for high hazard welding?"

**🤖 AI Agent:**
> Yes, a fire watch is required for high hazard welding, and they must remain on-site for the specified duration after the work is completed.

---

**👤 You:**
> "What is the exclusion zone for cutting with combustibles nearby?"

**🤖 AI Agent:**
> The required exclusion zone radius is 35 feet, and physical shielding is mandatory due to the presence of combustibles.

---

**👤 You:**
> "Do I need to monitor the air in a confined space for grinding?"

**🤖 AI Agent:**
> Yes, atmospheric monitoring is mandatory for confined spaces, and you must check for flammable gases and oxygen levels.


## ❓ FAQ

**Q: How do I determine if a fire watch is needed?**
You can use the `calculate_fire_watch` tool. It determines if a watch is required based on the hazard level and the type of operation being performed.

**Q: Can I calculate the safety perimeter for grinding?**
Yes, the `calculate_exclusion_zone` tool calculates the required radius in feet and whether physical shielding is mandatory for operations like grinding.

**Q: How is atmospheric safety handled?**
The `check_atmospheric_safety` tool evaluates if air testing is mandatory, especially for confined spaces, and identifies which gases must be monitored.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/hot-work-permit-system](https://vinkius.com/en/ai-agent-connect/hot-work-permit-system)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hot Work Permit System** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hot-work-permit-system` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hot Work Permit System** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hot-work-permit-system": {
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
