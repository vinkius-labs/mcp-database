# Truss Analysis Pro MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/truss-analysis-pro)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate internal forces, reactions, and deflection in truss structures.

## Description
This MCP server provides structural engineering tools to analyze truss structures. Use `analyze_truss_equilibrium` to find support reactions, `calculate_member_forces` to determine axial tension or compression, `estimate_max_deflection` to predict displacement, and `verify_structural_integrity` to check if members meet safety requirements.


## Available Tools (4)
- **calculate_member_forces**: Determines the axial tension or compression in every individual member of the truss
- **estimate_max_deflection**: Predicts the maximum displacement of the truss structure under the specified loading conditions
- **verify_structural_integrity**: Checks if the calculated forces exceed the capacity of the truss members
- **analyze_truss_equilibrium**: Calculates the external reaction forces at the supports based on the applied loads and truss geometry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Truss Analysis Pro** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the reaction forces for a Pratt truss with a 10m span and 2m height, with a 5kN load at 5m."

**🤖 AI Agent:**
> The vertical reaction forces are 2.5kN at the first support and 2.5kN at the second support.

---

**👤 You:**
> "What is the maximum deflection for a Warren truss, 20m span, 3m height, with a 10kN load at 10m, using steel (E=200GPa, A=500mm2)?"

**🤖 AI Agent:**
> The maximum deflection is 0.015 meters located at the 10m mark.

---

**👤 You:**
> "Check if a member with 50kN force and 40kN capacity is safe."

**🤖 AI Agent:**
> The member is overloaded with a utilization of 1.25.


## ❓ FAQ

**Q: What truss types are supported?**
The server supports standard configurations including Pratt, Warren, and Howe trusses.

**Q: How do I check if my truss is safe?**
You can use the `verify_structural_integrity` tool by providing the calculated member forces and their capacities.

**Q: Can I account for joint rigidity?**
Yes, when using `calculate_member_forces`, you can set the `includeSecondaryStresses` parameter to true to account for joint rigidity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/truss-analysis-pro](https://vinkius.com/ai-agent-connect/truss-analysis-pro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Truss Analysis Pro** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `truss-analysis-pro` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Truss Analysis Pro** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "truss-analysis-pro": {
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
