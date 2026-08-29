# Ceramic Formulation Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ceramic-formulation-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design ceramic batches and glazes by calculating oxide profiles, thermal expansion, and sintering temperatures.

## Description
This MCP server provides specialized tools for ceramic engineers to design precise material formulations. Use `calculate_batch_composition` to determine the exact raw material weights needed for a target oxide profile. Evaluate glaze-to-body fit using `calculate_glaze_compatibility` to prevent defects like crazing. Predict densification behavior with `predict_sintering_temperature` and calculate the Coefficient of Thermal Expansion (CTE) via `calculate_thermal_expansion` to ensure physical stability in ceramic products.


## Available Tools (4)
- **calculate_batch_composition**: Determines the necessary quantities of raw materials to achieve a specific target oxide profile
- **calculate_glaze_compatibility**: Evaluates if a proposed glaze formulation is chemically and physically compatible with a ceramic body
- **calculate_thermal_expansion**: Calculates the Coefficient of Thermal Expansion (CTE) for a given chemical formulation
- **predict_sintering_temperature**: Estimates the temperature at which a specific formulation will undergo significant densification


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ceramic Formulation Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the batch composition for a target profile of 60% SiO2 and 40% Al2O3 using Kaolin (45% SiO2, 45% Al2O3) and Quartz (95% SiO2)."

**🤖 AI Agent:**
> To achieve a 60/40 SiO2/Al2O3 profile, you need 80.0 units of Kaolin and 20.0 units of Quartz.

---

**👤 You:**
> "What is the thermal expansion for a mixture containing 70% SiO2 and 30% CaO?"

**🤖 AI Agent:**
> The calculated Coefficient of Thermal Expansion (CTE) for this formulation is 6.5 x 10^-6 /°C.

---

**👤 You:**
> "Predict the sintering temperature for a profile with 60% SiO2, 20% Al2O3, and 20% Na2O with a flux intensity of 0.8."

**🤖 AI Agent:**
> The estimated sintering temperature is 1150°C with a sintering range of 1120°C - 1180°C.


## ❓ FAQ

**Q: How do I calculate the raw materials needed for a specific recipe?**
Use the `calculate_batch_composition` tool. You must provide the target oxide profile (e.g., SiO2, Al2O3 percentages) and a list of your available raw materials.

**Q: Can I check if my glaze will crack on my ceramic body?**
Yes, use `calculate_glaze_compatibility` to compare the oxide profiles of your glaze and body. It will return a risk level and the CTE mismatch to help prevent crazing.

**Q: How is the sintering temperature estimated?**
The `predict_sintering_temperature` tool estimates densification temperatures based on the oxide profile and the concentration of fluxing agents present in the mix.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ceramic-formulation-calculator](https://vinkius.com/ai-agent-connect/ceramic-formulation-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ceramic Formulation Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ceramic-formulation-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ceramic Formulation Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ceramic-formulation-calculator": {
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
