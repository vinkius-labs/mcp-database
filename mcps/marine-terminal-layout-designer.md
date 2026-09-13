# Marine Terminal Layout Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/marine-terminal-layout-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Calculate berth requirements, jetty dimensions, and loading reach for marine terminals.

## Description
This MCP server provides essential engineering calculations for designing marine terminal infrastructure. It allows AI agents to determine necessary docking spaces using `get_berth_capacity`, calculate physical dimensions with `calculate_jetty_dimensions`, verify equipment reach via `calculate_loading_reach`, and ensure site compliance through `validate_site_feasibility`. It is designed to assist maritime engineers in planning vessel access, maneuvering areas, and jetty structures based on vessel types and cargo throughput.


## Available Tools (4)
- **calculate_jetty_dimensions**: Calculates the necessary physical length of the jetty and the required maneuvering space
- **calculate_loading_reach**: Determines if the proposed loading equipment can successfully reach the vessel's connection points
- **get_berth_capacity**: Determines how many docking spaces are required to meet specific cargo demands
- **validate_site_feasibility**: Checks if the proposed terminal layout fits within the physical constraints of the site


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Marine Terminal Layout Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many berths do I need for a Panamax vessel with an annual throughput of 5,000,000 tons and a 48-hour turnaround time?"

**🤖 AI Agent:**
> To handle 5,000,000 tons of Panamax cargo with a 48-hour turnaround, you will require 4 berths.

---

**👤 You:**
> "What is the required jetty length for 3 Supramax berths with a 10-meter safety margin?"

**🤖 AI Agent:**
> The total required jetty length for 3 Supramax berths with a 10-meter safety margin is 450 meters.

---

**👤 You:**
> "Will a Marine Loading Arm reach a VLCC if the jetty width is 15 meters?"

**🤖 AI Agent:**
> Yes, the Marine Loading Arm has an effective working range that successfully reaches the VLCC connection points at a jetty width of 15 meters.


## ❓ FAQ

**Q: How do I calculate the number of berths needed?**
You can use the `get_berth_capacity` tool by providing the vessel type, annual throughput, and average turnaround time.

**Q: Can I check if my jetty is long enough for a specific ship?**
Yes, use `calculate_jetty_dimensions` to determine the required length and maneuvering area for your chosen vessel type.

**Q: How do I verify if the terminal fits the site constraints?**
Use the `validate_site_feasibility` tool to check if your calculated jetty length and maneuvering area comply with your site's physical boundaries.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/marine-terminal-layout-designer](https://vinkius.com/en/ai-agent-connect/marine-terminal-layout-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Marine Terminal Layout Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `marine-terminal-layout-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Marine Terminal Layout Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "marine-terminal-layout-designer": {
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
