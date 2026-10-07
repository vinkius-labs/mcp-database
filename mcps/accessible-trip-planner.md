# Accessible Trip Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-trip-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Evaluates transport, lodging, and attractions against specific mobility and timing needs.

## Description
This MCP server provides specialized planning tools to identify compatible travel options for users with specific mobility requirements. It uses `get_transport_options` to find accessible transit routes, `get_lodging_options` to locate suitable accommodations, and `get_attraction_availability` to verify point-of-interest accessibility. Finally, `analyze_trip_feasibility` synthesizes these components into a comprehensive report to identify potential accessibility gaps.


## Available Tools (4)
- **analyze_trip_feasibility**: Synthesize transport, lodging, and attractions into a single feasibility report
- **get_attraction_availability**: Check if specific points of interest can be visited given mobility and timing constraints
- **get_lodging_options**: Identify hotels or stays that accommodate specific accessibility and companion needs
- **get_transport_options**: Find available transit routes that match a user's mobility profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Trip Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find accessible transport from London to Oxford for a wheelchair user."

**🤖 AI Agent:**
> The available route via rail includes step-free access at both stations and low-floor boarding, making it feasible for a wheelchair user.

---

**👤 You:**
> "Is the Eiffel Tower accessible for someone with limited mobility?"

**🤖 AI Agent:**
> Yes, the Eiffel Tower provides elevator access and step-free paths suitable for users with limited mobility.

---

**👤 You:**
> "Check if my trip plan is feasible for a user requiring a companion."

**🤖 AI Agent:**
> The trip is feasible. All selected transport, lodging, and attractions provide the necessary support for a traveler requiring a companion.


## ❓ FAQ

**Q: How does the tool handle different mobility needs?**
The server uses standardized mobility profiles like `wheelchair_user` or `visual_impairment` to filter all transport, lodging, and attraction options.

**Q: Can I check if a specific hotel is accessible?**
Yes, you can use `get_lodging_options` to find accommodations that match your specific mobility profile and companion requirements.

**Q: What is a critical gap?**
A critical gap is a fundamental mismatch in a mobility requirement, such as a lack of wheelchair access when a user requires it, identified during `analyze_trip_feasibility`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-trip-planner](https://vinkius.com/en/ai-agent-connect/accessible-trip-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Trip Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-trip-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Trip Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-trip-planner": {
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
