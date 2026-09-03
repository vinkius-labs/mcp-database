# Concrete Two-Way Slab Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-two-way-slab-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Automated ACI-compliant design for two-way reinforced concrete slabs.

## Description
This MCP server provides specialized engineering tools for designing two-way reinforced concrete slabs according to ACI provisions. It allows AI agents to perform critical structural calculations including `calculate_slab_thickness` to ensure deflection and punching shear compliance, `distribute_moments` for determining bending distributions using direct design or equivalent frame methods, `design_reinforcement` for steel layout, and `evaluate_support_details` to determine the need for drop panels and column capitals.


## Available Tools (4)
- **calculate_slab_thickness**: Determines the required minimum slab thickness to satisfy deflection and punching shear requirements
- **design_reinforcement**: Determines the required area and spacing of steel reinforcement
- **distribute_moments**: Calculates the negative and positive bending moments across the slab panel
- **evaluate_support_details**: Evaluates the necessity and dimensions of column capitals and drop panels


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Two-Way Slab Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the required thickness for a slab with a 5m span, 30MPa concrete, and a 10kN/m² load."

**🤖 AI Agent:**
> The minimum required slab thickness is 150 mm, and it satisfies the punching shear requirements.

---

**👤 You:**
> "What are the bending moments for a 6m x 4m slab using the direct design method with a 12kN/m² load?"

**🤖 AI Agent:**
> The negative moments at the supports are 45.5 kNm and the positive moments in the mid-span are 22.8 kNm.

---

**👤 You:**
> "Determine the reinforcement layout for a slab with positive moment of 15 kNm, negative moment of 25 kNm, 180mm thickness, 30MPa concrete, and 420MPa steel."

**🤖 AI Agent:**
> The required reinforcement uses 12mm diameter bars spaced at 150mm.


## ❓ FAQ

**Q: Which design methods are supported?**
The server supports both the Direct Design Method and the Equivalent Frame Method for moment distribution.

**Q: How is slab thickness determined?**
The `calculate_slab_thickness` tool uses ACI span-to-effective-depth ratios to ensure the slab meets deflection and punching shear requirements.

**Q: Can I check for punching shear requirements?**
Yes, the thickness calculation includes a check to verify if the slab satisfies punching shear requirements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-two-way-slab-designer](https://vinkius.com/ai-agent-connect/concrete-two-way-slab-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Two-Way Slab Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-two-way-slab-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Two-Way Slab Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-two-way-slab-designer": {
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
