# Sand Separation Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sand-separation-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Engineering tools for designing desanders and hydrocyclones based on fluid dynamics.

## Description
This MCP server provides specialized engineering tools for designing sand separation systems. It allows users to calculate desander dimensions, evaluate hydrocyclone capacity, assess erosion risk, and optimize overall system configurations. By applying principles like Stokes' law, the tools help determine the necessary equipment to handle specific sand production rates and particle size distributions in oil, gas, and water treatment processes.


## Available Tools (4)
- **assess_erosion_risk**: Predict wear and tear on separation equipment based on sand characteristics
- **calculate_desander_dimensions**: Determine the physical size and configuration of a desander vessel
- **evaluate_hydrocyclone_capacity**: Determine if a hydrocyclone configuration can handle current sand production and fluid flow
- **optimize_system_configuration**: Recommend a combination of desander and hydrocyclone components


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sand Separation Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the desander dimensions for a flow rate of 500 m3/h, sand production of 5 kg/h, minimum particle size of 0.05 mm, and fluid viscosity of 0.001 Pa·s."

**🤖 AI Agent:**
> The required desander vessel has a diameter of 1.2 meters, a height of 3.5 meters, and a residence time of 45 seconds with a capture efficiency of 98%.

---

**👤 You:**
> "What is the erosion risk for a fluid velocity of 5 m/s with a sand production rate of 10 kg/h and a particle size distribution of {'0.05': 0.5, '0.1': 0.5} using carbon steel?"

**🤖 AI Agent:**
> The predicted erosion rate is 0.15 mm/year, resulting in a high risk level and an expected lifespan of 4.2 years for the carbon steel liner.

---

**👤 You:**
> "Recommend a system configuration for a target flow rate of 1000 m3/h and sand production of 20 kg/h with a minimum particle capture size of 0.03 mm."

**🤖 AI Agent:**
> The recommended configuration includes 2 desanders and a high-efficiency hydrocyclone, with a total estimated footprint of 15 m2 and an estimated efficiency of 99.2%.


## ❓ FAQ

**Q: How do I calculate the size of a desander?**
You can use the `calculate_desander_dimensions` tool. Provide the sand production rate, fluid flow rate, minimum particle size, and fluid viscosity to receive the vessel diameter, height, and residence time.

**Q: Can I predict equipment wear from sand?**
Yes, the `assess_erosion_risk` tool predicts the erosion rate and expected lifespan of your equipment based on sand production, particle size distribution, fluid velocity, and material hardness.

**Q: How do I check if a hydrocyclone is sufficient?**
Use the `evaluate_hydrocyclone_capacity` tool. It checks if a specific hydrocyclone diameter can handle the sand production and fluid flow while maintaining capture efficiency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sand-separation-design](https://vinkius.com/en/ai-agent-connect/sand-separation-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sand Separation Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sand-separation-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sand Separation Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sand-separation-design": {
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
