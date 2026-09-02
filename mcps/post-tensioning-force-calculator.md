# Post-Tensioning Force Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/post-tensioning-force-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculates post-tensioning requirements including jacking force, tendon geometry, and elongation.

## Description
This MCP server provides specialized engineering tools for post-tensioning design in concrete slabs using the Load Balancing Method. It allows AI agents to perform complex structural calculations, including determining the `calculate_jacking_force` to account for friction and anchorage losses, calculating `determine_tendon_geometry` for spacing and area, predicting `calculate_elongation` for field verification, and performing `verify_design_safety` to ensure compatibility with concrete strength.


## Available Tools (4)
- **calculate_elongation**: Predicts the physical stretch of the tendon to allow for field verification
- **verify_design_safety**: Validates if the calculated post-tensioning requirements are compatible with the concrete strength
- **calculate_jacking_force**: Determines the total initial force required to overcome losses and achieve the target balancing force
- **determine_tendon_geometry**: Calculates the physical dimensions and placement of the tendons within the slab


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Post-Tensioning Force Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the jacking force for a 10m span slab, 250mm thick, with 15 kN/m² load and 30 MPa concrete using a parabolic profile."

**🤖 AI Agent:**
> The required jacking force is 450.5 kN with an effective force of 425.2 kN after accounting for losses.

---

**👤 You:**
> "What is the expected elongation for a tendon with 500 kN jacking force, 150 mm² area, and 12m length with a modulus of 200000 MPa?"

**🤖 AI Agent:**
> The predicted elongation for the tendon is 45.0 mm.

---

**👤 You:**
> "Check if a design with 35 MPa concrete, 400 kN jacking force, and 200mm slab thickness is safe."

**🤖 AI Agent:**
> The design is safe with a reserve capacity of 12.5 MPa.


## ❓ FAQ

**Q: What is the Load Balancing Method used here?**
It is a design approach where the tendon profile is shaped to create upward pressure that offsets a portion of the downward gravity loads.

**Q: How does the tool handle friction losses?**
The `calculate_jacking_force` tool includes an optional parameter to account for the friction coefficient between the tendon and the duct.

**Q: Can I verify if my design is safe?**
Yes, you can use the `verify_design_safety` tool to check if the induced compressive stresses are within the limits of your concrete strength.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/post-tensioning-force-calculator](https://vinkius.com/ai-agent-connect/post-tensioning-force-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Post-Tensioning Force Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `post-tensioning-force-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Post-Tensioning Force Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "post-tensioning-force-calculator": {
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
