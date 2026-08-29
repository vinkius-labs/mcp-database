# Adsorption Isotherm Fitting MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/adsorption-isotherm-fitting)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Mathematical modeling for adsorption isotherms including Langmuir and Freundlich models.

## Description
This MCP server provides specialized mathematical tools to analyze adsorption processes. It allows users to fit experimental data to standard models like `fit_langmuir_isotherm` for monolayer adsorption or `fit_freundlich_isotherm` for multilayer/heterogeneous surfaces. Users can also use `compare_isotherm_models` to determine the best fit based on R-squared values and `calculate_adsorption_efficiency` to evaluate removal performance. It serves as a bridge between experimental chemical data and precise mathematical characterization.


## Available Tools (4)
- **calculate_adsorption_efficiency**: Evaluates how effectively a specific adsorbent removes a substance from a solution at a given concentration
- **compare_isotherm_models**: Evaluates which of the primary models (Langmuir or Freundlich) provides the best fit for a specific dataset
- **fit_freundlich_isotherm**: Determines if the data follows a multilayer or heterogeneous surface adsorption pattern using the Freundlich model
- **fit_langmuir_isotherm**: Determines if the data follows a single-layer adsorption pattern using the Langmuir model


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Adsorption Isotherm Fitting** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare Langmuir and Freundlich models for these data points: [{'equilibriumConcentration': 10, 'adsorbedAmount': 5}, {'equilibriumConcentration': 20, 'adsorbedAmount': 12}]"

**🤖 AI Agent:**
> The Langmuir model is the best fit for this dataset with an R-squared of 0.98.

---

**👤 You:**
> "Calculate the adsorption efficiency if the initial concentration was 100 mg/L, the equilibrium concentration is 10 mg/L, the adsorbed amount is 5 mg/g, the adsorbent mass is 1g, and the volume is 1L."

**🤖 AI Agent:**
> The removal percentage is 90% and the mass transfer ratio is 5.0.

---

**👤 You:**
> "Fit a Langmuir isotherm to these points: [{'equilibriumConcentration': 5, 'adsorbedAmount': 2}, {'equilibriumConcentration': 15, 'adsorbedAmount': 6}]"

**🤖 AI Agent:**
> The Langmuir fit results in a maximum capacity of 10.0 and an affinity constant of 0.15.


## ❓ FAQ

**Q: How do I know which model fits my data best?**
You can use the `compare_isotherm_models` tool, which evaluates both Langmuir and Freundlich models and identifies the best fit based on the highest R-squared value.

**Q: Can I calculate removal efficiency directly?**
Yes, the `calculate_adsorption_efficiency` tool calculates the removal percentage and the mass transfer ratio using your concentration and mass data.

**Q: What kind of data is required for fitting?**
The tools require an array of data points, where each point contains the equilibrium concentration and the adsorbed amount.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/adsorption-isotherm-fitting](https://vinkius.com/ai-agent-connect/adsorption-isotherm-fitting)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Adsorption Isotherm Fitting** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `adsorption-isotherm-fitting` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Adsorption Isotherm Fitting** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "adsorption-isotherm-fitting": {
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
