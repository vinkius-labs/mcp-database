# Concrete Joint Spacing Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-joint-spacing-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculates optimal contraction joint spacing, depth, and sealant requirements for concrete slabs.

## Description
This MCP server provides precise engineering calculations for concrete slab contraction joints. It helps engineers and contractors determine the ideal horizontal distance between joints using `calculate_optimal_spacing` to prevent uncontrolled cracking. It also calculates necessary cut depths with `determine_joint_geometry`, estimates material needs via `estimate_sealant_needs`, and verifies structural integrity using `analyze_load_transfer_capacity`.


## Available Tools (4)
- **analyze_load_transfer_capacity**: Evaluates if the proposed joint geometry provides sufficient load transfer across the joint
- **calculate_optimal_spacing**: Determines the ideal horizontal distance between contraction joints to prevent uncontrolled cracking
- **determine_joint_geometry**: Calculates the required depth of the contraction cut based on the slab thickness and structural needs
- **estimate_sealant_needs**: Calculates the amount of sealant required to fill the joints for a specific project area


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Joint Spacing Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the optimal spacing for a 200mm thick slab with standard concrete and 1% reinforcement?"

**🤖 AI Agent:**
> The optimal joint spacing for a 200mm slab with standard concrete and 1% reinforcement is 3.5 meters.

---

**👤 You:**
> "How much sealant do I need for a 500 square meter slab with 3 meter spacing and 40mm deep joints?"

**🤖 AI Agent:**
> For a 500 square meter slab, you will need approximately 166.67 linear meters of sealant and 6.67 liters of sealant volume.

---

**👤 You:**
> "Is a 50mm joint depth adequate for a 250mm slab with 2% reinforcement?"

**🤖 AI Agent:**
> Yes, the load transfer capacity is adequate for these parameters.


## ❓ FAQ

**Q: How do I determine the spacing between joints?**
You can use the `calculate_optimal_spacing` tool. Provide the slab thickness, concrete type, reinforcement ratio, base friction, and the expected temperature range.

**Q: Can I estimate sealant volume?**
Yes, the `estimate_sealant_needs` tool calculates both the total linear meters and the total volume in liters required for your specific slab area and joint dimensions.

**Q: How is load transfer capacity assessed?**
The `analyze_load_transfer_capacity` tool evaluates the remaining un-cut thickness of the slab against the reinforcement density to ensure structural stability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-joint-spacing-calculator](https://vinkius.com/ai-agent-connect/concrete-joint-spacing-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Joint Spacing Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-joint-spacing-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Joint Spacing Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-joint-spacing-calculator": {
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
