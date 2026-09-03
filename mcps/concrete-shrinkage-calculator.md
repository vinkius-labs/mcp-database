# Concrete Shrinkage Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-shrinkage-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Predict concrete shrinkage strain, physical deformation, and optimal joint spacing using the ACI 209 model.

## Description
This MCP server provides structural engineering tools to predict concrete shrinkage behavior. It uses the ACI 209 model to calculate shrinkage strain based on environmental factors like humidity and material properties like cement and aggregate types. Engineers can use `get_shrinkage_strain` to find the strain value, `get_deformation_mm` to calculate physical length changes, and `get_recommended_joint_spacing` to determine the best distance between control joints to prevent cracking. It also includes `get_material_properties` for looking up specific shrinkage coefficients.


## Available Tools (4)
- **get_recommended_joint_spacing**: Determine optimal distance between joints to prevent shrinkage cracks
- **get_deformation_mm**: Calculate the physical change in length (deformation) of a concrete member
- **get_material_properties**: Retrieve standardized shrinkage coefficients for specific material combinations
- **get_shrinkage_strain**: Calculate predicted shrinkage strain based on environmental and material factors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Shrinkage Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the shrinkage strain for concrete that is 28 days old, in 50% humidity, with a thickness of 200mm, using Standard cement and Fine aggregate."

**🤖 AI Agent:**
> The predicted shrinkage strain is 0.00045.

---

**👤 You:**
> "What is the recommended joint spacing for a concrete member with a shrinkage strain of 0.0005, a thickness of 150mm, and a compressive strength of 30 MPa?"

**🤖 AI Agent:**
> The maximum recommended joint spacing is 3500 mm, with a Low risk level.

---

**👤 You:**
> "How much will a 5000mm long concrete beam deform if the shrinkage strain is 0.0004 and the restraint factor is 0.3?"

**🤖 AI Agent:**
> The total deformation is 2.0 mm, and the restrained deformation is 1.4 mm.


## ❓ FAQ

**Q: What model is used for these calculations?**
The server uses the ACI 209 shrinkage prediction model to calculate strain and deformation.

**Q: How do I calculate the physical deformation in millimeters?**
You can use the `get_deformation_mm` tool by providing the calculated shrinkage strain and the total length of the concrete member.

**Q: Can I account for reinforcement restraint?**
Yes, the `get_deformation_mm` tool accepts an optional restraint factor to account for internal reinforcement.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-shrinkage-calculator](https://vinkius.com/ai-agent-connect/concrete-shrinkage-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Shrinkage Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-shrinkage-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Shrinkage Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-shrinkage-calculator": {
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
