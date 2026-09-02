# Concrete Corbel Design Tool MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-corbel-design-tool)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate structural reinforcement, shear friction, and bearing capacity for concrete corbels.

## Description
This MCP server provides specialized engineering tools for designing concrete corbels. It calculates primary reinforcement using `calculate_flexural_requirements`, evaluates shear and interface stability with `calculate_shear_and_friction`, and verifies bearing pressure via `calculate_bearing_capacity`. Finally, `verify_design_integrity` ensures the complete design meets structural requirements and anchorage needs. It is designed for structural engineers to handle complex vertical and horizontal loading conditions.


## Available Tools (4)
- **calculate_flexural_requirements**: Determines the necessary steel reinforcement to resist bending moments
- **calculate_shear_and_friction**: Evaluates the need for shear reinforcement and validates the interface stability
- **verify_design_integrity**: Performs a holistic check of the calculated reinforcement against the geometry
- **calculate_bearing_capacity**: Checks if the bearing area is sufficient to prevent concrete crushing under the load


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Corbel Design Tool** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the reinforcement needed for a corbel with a 50kN vertical load, 10kN horizontal force, 200mm width, 400mm depth, 50mm eccentricity, 30MPa concrete, and 400MPa steel."

**🤖 AI Agent:**
> The required primary reinforcement area is 450 mm² with an anchorage length of 120 mm.

---

**👤 You:**
> "Check the bearing capacity for a 100kN load on a corbel that is 300mm wide and 300mm deep with 25MPa concrete."

**🤖 AI Agent:**
> The bearing pressure is 1.11 MPa, which is within the safe limits for 25MPa concrete.

---

**👤 You:**
> "Evaluate the shear and friction for a corbel with 60kN vertical load and 20kN horizontal force, 250mm width and 450mm depth, using 30MPa concrete and 400MPa steel."

**🤖 AI Agent:**
> The required shear reinforcement area is 115 mm² and the friction resistance is sufficient for the horizontal load.


## ❓ FAQ

**Q: How does the tool handle horizontal forces?**
The `calculate_flexural_requirements` tool accounts for the additional moment created by the horizontal force, ensuring the primary reinforcement is sufficient for combined loading.

**Q: Can I verify if my corbel design is safe?**
Yes, you can use `verify_design_integrity` to perform a holistic check of reinforcement, anchorage length, and safety margins.

**Q: Does this tool check for concrete crushing?**
Yes, `calculate_bearing_capacity` checks if the bearing area is sufficient to prevent local crushing of the concrete under the applied vertical load.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-corbel-design-tool](https://vinkius.com/ai-agent-connect/concrete-corbel-design-tool)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Corbel Design Tool** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-corbel-design-tool` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Corbel Design Tool** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-corbel-design-tool": {
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
