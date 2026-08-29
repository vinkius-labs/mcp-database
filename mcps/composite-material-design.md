# Composite Material Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/composite-material-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate mechanical properties, optimal fiber content, and laminate stiffness for composite materials.

## Description
This MCP server provides specialized tools for composite mechanics and material design. Use `calculate_composite_properties` to determine longitudinal and transverse moduli based on volume fractions. Use `optimize_fiber_fraction` to find the exact reinforcement needed for a target stiffness. For multi-layer structures, `calculate_laminate_stiffness` predicts effective stiffness based on ply orientations, while `validate_material_compatibility` ensures density constraints are met.


## Available Tools (4)
- **calculate_composite_properties**: Determines the theoretical mechanical properties of a single-phase composite based on a specific volume fraction
- **calculate_laminate_stiffness**: Predicts the effective stiffness of a multi-layer laminate given different ply orientations
- **optimize_fiber_fraction**: Finds the specific volume fraction of reinforcement required to meet a target stiffness
- **validate_material_compatibility**: Checks if a specific reinforcement and matrix combination is physically viable for a design


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Composite Material Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the properties of a composite with a matrix modulus of 3 GPa, reinforcement modulus of 230 GPa, Poisson ratio of 0.3 for both, and a 60% fiber volume fraction."

**🤖 AI Agent:**
> The longitudinal modulus is 139.2 GPa, the transverse modulus is 3.3 GPa, and the effective Poisson ratio is 0.3.

---

**👤 You:**
> "What fiber fraction is needed to achieve a target modulus of 100 GPa if the matrix is 3 GPa and reinforcement is 230 GPa?"

**🤖 AI Agent:**
> The optimal fiber fraction required to achieve a 100 GPa modulus is approximately 0.422.

---

**👤 You:**
> "Check if a composite with matrix density 1.2 and reinforcement density 1.8 is viable for a max weight of 1.5."

**🤖 AI Agent:**
> The calculated density is 1.56, which exceeds the maximum allowable weight of 1.5. The material is not viable.


## ❓ FAQ

**Q: How do I calculate the stiffness of a composite?**
You can use the `calculate_composite_properties` tool to find the longitudinal and transverse modulus using the rule of mixtures.

**Q: Can I design multi-layer laminates?**
Yes, use `calculate_laminate_stiffness` to predict the effective stiffness of a stack of layers with specific orientations.

**Q: How do I find the right amount of fiber for a target stiffness?**
The `optimize_fiber_fraction` tool calculates the specific volume fraction required to reach your target modulus.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/composite-material-design](https://vinkius.com/ai-agent-connect/composite-material-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Composite Material Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `composite-material-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Composite Material Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "composite-material-design": {
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
