# Urea Plant Design Engineer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/urea-plant-design-engineer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Specialized engineering tool for urea production plant design and feedstock validation.

## Description
This MCP server provides specialized chemical engineering tools for designing urea production facilities. It allows engineers to use `calculate_reactor_specs` to determine physical reactor requirements, `calculate_recycle_requirements` to manage unreacted gas recovery, and `design_finishing_system` to select between prilling or granulation processes. It also includes `validate_feedstock_balance` to ensure ammonia and CO2 supplies meet stoichiometric needs for technologies like Stamicarbon, Snamprogetti, or ACES.


## Available Tools (4)
- **calculate_reactor_specs**: Determines the physical and operating requirements of the urea synthesis reactor
- **calculate_recycle_requirements**: Calculates the volume of unreacted gases that must be recovered and returned to the system
- **design_finishing_system**: Selects and specifies the appropriate equipment for converting liquid urea to solid product
- **validate_feedstock_balance**: Verifies if the provided ammonia and carbon dioxide levels can sustain the desired plant capacity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Urea Plant Design Engineer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the reactor specifications for a 1000 ton/day plant using Stamicarbon technology."

**🤖 AI Agent:**
> The required reactor volume is 45 cubic meters with an operating pressure of 150 bar and temperature of 185°C.

---

**👤 You:**
> "What is the recycle requirement for a reactor with 50 cubic meters volume using Snamprogetti at 0.6 conversion rate?"

**🤖 AI Agent:**
> The recycle ratio is 0.4 and the estimated recycle flow rate is 120 metric tons per day.

---

**👤 You:**
> "Design a granulation system for a 500 ton/day urea plant using ACES technology."

**🤖 AI Agent:**
> The granulation system requires a rotating drum with a capacity of 500 tons/day and a medium energy intensity profile.


## ❓ FAQ

**Q: Which process technologies are supported?**
The server supports Stamicarbon, Snamprogetti, and ACES process architectures.

**Q: Can I design the solid product system?**
Yes, you can use `design_finishing_system` to specify either prilling or granulation equipment based on your capacity requirements.

**Q: How do I check if my feedstock is sufficient?**
Use the `validate_feedstock_balance` tool to verify if your ammonia and CO2 supplies meet the stoichiometric requirements for your target capacity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/urea-plant-design-engineer](https://vinkius.com/en/ai-agent-connect/urea-plant-design-engineer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Urea Plant Design Engineer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `urea-plant-design-engineer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Urea Plant Design Engineer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "urea-plant-design-engineer": {
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
