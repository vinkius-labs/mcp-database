# Visbreaker Unit Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/visbreaker-unit-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemical-engineering](../categories/chemical-engineering.md)

Design visbreaker units for viscosity reduction using atmospheric residue properties.

## Description
This MCP server provides specialized tools for designing visbreaker units in petroleum refining. It allows AI agents to calculate necessary conversion metrics, simulate reactor operating conditions, evaluate the tradeoff between cracking severity and fuel stability, and predict final product quality. By using `get_conversion_metrics`, `simulate_operating_conditions`, `evaluate_severity_tradeoff`, and `calculate_product_quality`, engineers can optimize the viscosity reduction process while managing fouling tendencies.


## Available Tools (4)
- **calculate_product_quality**: Predict the final properties of the heavy residue after the visbreaking process
- **evaluate_severity_tradeoff**: Analyze the balance between the intensity of cracking and the quality of the resulting fuel
- **get_conversion_metrics**: Determine the necessary conversion and product distribution required to reach a specific viscosity target
- **simulate_operating_conditions**: Identify the temperature and residence time needed to achieve a specific conversion level


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Visbreaker Unit Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What conversion and yields do I need to reach a target viscosity of 15 cSt with this feedstock?"

**🤖 AI Agent:**
> To reach a target viscosity of 15 cSt, the required conversion is 25%, resulting in a gas yield of 2%, naphtha yield of 8%, light oil yield of 15%, and a heavy residue yield of 75%.

---

**👤 You:**
> "What are the operating conditions for a 30% conversion level?"

**🤖 AI Agent:**
> For a 30% conversion level, the required reactor temperature is 485°C, the residence time is 45 minutes, and the reactor pressure is 2.5 bar.

---

**👤 You:**
> "Analyze the tradeoff for a 40% conversion."

**🤖 AI Agent:**
> At 40% conversion, the severity index is 7.2, the stability score is 45/100, and the fouling tendency score is 65/100.


## ❓ FAQ

**Q: How can I determine the required conversion for a specific viscosity?**
You can use the `get_conversion_metrics` tool by providing the feedstock properties and your target viscosity.

**Q: Does this tool help manage the stability vs. fouling tradeoff?**
Yes, the `evaluate_severity_tradeoff` tool specifically analyzes the balance between cracking intensity and the resulting fuel quality, including stability and fouling tendency.

**Q: Can I predict the final residue properties?**
Yes, the `calculate_product_quality` tool predicts final viscosity, density, sulfur content, and fouling tendency based on the planned conversion.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/visbreaker-unit-design](https://vinkius.com/en/ai-agent-connect/visbreaker-unit-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Visbreaker Unit Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `visbreaker-unit-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Visbreaker Unit Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "visbreaker-unit-design": {
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
