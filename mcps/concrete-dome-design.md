# Concrete Dome Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-dome-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Structural analysis for concrete thin-shell dome structures.

## Description
This MCP server provides specialized structural engineering tools for designing concrete thin-shell domes. It uses membrane theory to calculate critical dimensions and stability. Use `calculate_shell_thickness` to determine required thickness, `calculate_reinforcement` for steel requirements, `calculate_support_forces` for base reactions, and `validate_stability` to check for buckling risks.


## Available Tools (4)
- **calculate_shell_thickness**: Determines the required concrete thickness to satisfy both material strength and buckling stability
- **calculate_support_forces**: Calculates the reaction forces at the base of the dome
- **calculate_reinforcement**: Determines the amount of steel reinforcement needed to handle tensile stresses and prevent cracking
- **validate_stability**: Evaluates if a designed dome is at risk of sudden collapse due to buckling or imperfections


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Dome Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the required thickness for a 20m diameter dome with a 5m rise, 10 kN/m² load, and 30 MPa concrete?"

**🤖 AI Agent:**
> The required thickness is 120 mm with a buckling safety factor of 2.4.

---

**👤 You:**
> "Calculate the support forces for a 15m diameter dome, 4m rise, 5 kN/m² load, using a pinned support."

**🤖 AI Agent:**
> The vertical reaction is 441.78 kN and the horizontal thrust is 147.26 kN.

---

**👤 You:**
> "How much steel reinforcement is needed for a 10m diameter, 3m rise dome with 8 kN/m² load and 100mm thickness using 25 MPa concrete?"

**🤖 AI Agent:**
> The required meridional steel area is 450 mm² and the hoop steel area is 320 mm², with a suggested maximum spacing of 250 mm.


## ❓ FAQ

**Q: How do I determine the required thickness for my dome?**
You can use the `calculate_shell_thickness` tool. Provide the diameter, rise, design load, and concrete strength to get the minimum thickness in mm and the buckling safety factor.

**Q: Can I check if my design is stable against buckling?**
Yes, the `validate_stability` tool evaluates if your design meets safety margins by comparing the design load against the calculated buckling capacity.

**Q: What kind of support conditions are supported?**
The tool supports both 'pinned' and 'fixed' support conditions via the `calculate_support_forces` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-dome-design](https://vinkius.com/ai-agent-connect/concrete-dome-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Dome Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-dome-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Dome Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-dome-design": {
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
