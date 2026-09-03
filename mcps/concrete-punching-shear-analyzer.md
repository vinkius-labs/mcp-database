# Concrete Punching Shear Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-punching-shear-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Evaluates punching shear capacity and stud rail requirements for concrete slabs using ACI standards.

## Description
This MCP server provides structural engineering tools to analyze punching shear in concrete slabs. It allows AI agents to calculate shear stress, evaluate concrete capacity, and design reinforcement requirements. Use `calculate_shear_stress` to find the critical perimeter and stress, `evaluate_capacity` to check if the slab meets ACI standards, and `design_stud_rails` to determine necessary reinforcement when capacity is exceeded. It also includes `account_for_openings` to adjust calculations for slab penetrations.


## Available Tools (4)
- **evaluate_capacity**: Compares the applied shear stress against the concrete's shear capacity to determine if reinforcement is needed
- **account_for_openings**: Adjusts the critical perimeter and stress calculations to account for slab penetrations
- **design_stud_rails**: 0 and you need to design stud rail reinforcement.

Provides the necessary reinforcement requirements if the slab fails the punching shear check
- **calculate_shear_stress**: Determines the current shear stress acting on the slab at the critical section


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Punching Shear Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the punching shear stress for a 300x300mm column on a 200mm thick slab with an effective depth of 170mm and a 500kN load."

**🤖 AI Agent:**
> The punching shear stress is 0.45 MPa and the critical perimeter is 1280 mm.

---

**👤 You:**
> "If the shear stress is 1.5 MPa and the concrete strength is 30 MPa with a reinforcement ratio of 0.01, does the slab need stud rails?"

**🤖 AI Agent:**
> Yes, the capacity utilization is 1.25, which exceeds the limit, so stud rails are required.

---

**👤 You:**
> "How many studs are needed for a 200mm thick slab with a 300mm column width if capacity utilization is 1.3?"

**🤖 AI Agent:**
> The design requires 12 studs with a recommended spacing of 150 mm.


## ❓ FAQ

**Q: How do I check if my slab needs reinforcement?**
Run `calculate_shear_stress` to get the stress, then use `evaluate_capacity`. If the capacity utilization is greater than 1.0, the slab requires reinforcement.

**Q: Can this tool account for slab openings?**
Yes, use the `account_for_openings` tool to adjust the critical perimeter and stress factors based on the dimensions and location of the opening.

**Q: What standards does this follow?**
The calculations follow ACI punching shear provisions for concrete slab design.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-punching-shear-analyzer](https://vinkius.com/ai-agent-connect/concrete-punching-shear-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Punching Shear Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-punching-shear-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Punching Shear Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-punching-shear-analyzer": {
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
