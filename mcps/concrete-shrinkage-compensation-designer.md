# Concrete Shrinkage Compensation Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-shrinkage-compensation-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Design shrinkage-compensating concrete by calculating expansive cement content and reinforcement needs.

## Description
This MCP server provides technical tools to design concrete elements that counteract drying and autogenous shrinkage. It uses Type K cement expansion calculations to determine the required expansive cement mass per cubic meter. Users can evaluate physical constraints using `analyze_restraint_risks`, adjust parameters for environmental factors with `simulate_environmental_impact`, and determine necessary steel reinforcement via `design_reinforcement`. It is a specialized tool for structural engineers to mitigate cracking risks in concrete structures.


## Available Tools (4)
- **analyze_restraint_risks**: Evaluates how much the physical constraints of the element will exacerbate shrinkage-induced stress
- **calculate_expansive_content**: Determines the mass of expansive cement needed per cubic meter to achieve the target compensation
- **design_reinforcement**: Calculates the necessary steel reinforcement to manage residual stresses and crack widths
- **simulate_environmental_impact**: Adjusts the shrinkage and expansion parameters based on ambient environmental conditions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Shrinkage Compensation Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much expansive cement do I need for a C30/37 concrete with 0.0005 shrinkage strain and a Type K factor of 0.02 in normal moisture?"

**🤖 AI Agent:**
> The required expansive cement content is 25.0 kg/m³ to achieve the target expansion strain.

---

**👤 You:**
> "What is the crack risk for a slab 5m x 5m x 0.2m with a restraint level of 0.8 and C30/37 grade?"

**🤖 AI Agent:**
> The crack risk level is High, with a restraint stress index of 24.0.

---

**👤 You:**
> "Adjust a shrinkage strain of 0.0004 for 35 degrees Celsius and 40% humidity."

**🤖 AI Agent:**
> The adjusted shrinkage strain is 0.00052 due to increased temperature and lower humidity.


## ❓ FAQ

**Q: How do I calculate the required additive amount?**
Use the `calculate_expansive_content` tool by providing the expected shrinkage strain, concrete grade, and the Type K expansion factor.

**Q: Can I account for weather conditions?**
Yes, the `simulate_environmental_impact` tool allows you to adjust shrinkage estimates based on ambient temperature and relative humidity.

**Q: How is reinforcement determined?**
The `design_reinforcement` tool calculates the required steel area based on the balance between expansion strain, shrinkage strain, and the restraint stress index.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-shrinkage-compensation-designer](https://vinkius.com/ai-agent-connect/concrete-shrinkage-compensation-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Shrinkage Compensation Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-shrinkage-compensation-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Shrinkage Compensation Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-shrinkage-compensation-designer": {
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
