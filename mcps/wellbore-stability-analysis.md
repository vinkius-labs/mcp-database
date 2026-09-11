# Wellbore Stability Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wellbore-stability-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Predict drilling safety windows by calculating mechanical integrity against formation stresses and pore pressures.

## Description
This MCP server provides specialized tools for drilling engineers to maintain borehole integrity. It calculates the critical mud weight window by balancing hydrostatic pressure against in-situ stresses. Use `calculate_stability_window` to determine the safe operating range between collapse and fracture pressures. You can also use `evaluate_time_dependent_risk` to predict how rock strength changes over time, or `calculate_collapse_pressure` to find the minimum pressure needed to prevent wellbore crushing. For chemical considerations, `analyze_chemical_interaction` estimates how fluid types like water-based or oil-based muds affect rock properties.


## Available Tools (4)
- **calculate_collapse_pressure**: Specifically calculates the minimum pressure required to maintain borehole stability against crushing
- **calculate_stability_window**: Determines the safe operating range for mud weight to prevent both collapse and fracturing
- **analyze_chemical_interaction**: Estimates the impact of drilling fluid chemistry on the near-wellbore rock properties
- **evaluate_time_dependent_risk**: Predicts how rock strength and stability change over time due to environmental factors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wellbore Stability Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the safe mud weight window for a vertical well with 40 MPa vertical stress, 30 MPa min horizontal stress, 35 MPa max horizontal stress, 25 MPa pore pressure, 50 MPa UCS, and 1200 kg/m³ mud weight?"

**🤖 AI Agent:**
> The safe mud weight window is 15.5 MPa, with a collapse pressure of 32.2 MPa and a fracture pressure of 47.7 MPa.

---

**👤 You:**
> "How much will the rock strength degrade after 24 hours if the initial strength is 45 MPa and the degradation rate is 0.1 per hour in shale?"

**🤖 AI Agent:**
> The remaining strength is 21.6 MPa, representing a 52% degradation, and the stability status is critical.

---

**👤 You:**
> "What is the impact of using water-based mud on shale with a salinity of 5?"

**🤖 AI Agent:**
> The strength reduction factor is 0.85, with a high swelling potential of 0.75, leading to increased permeability in the near-wellbore region.


## ❓ FAQ

**Q: How do I find the safe mud weight range?**
You can use the `calculate_stability_window` tool. Provide the in-situ stresses, pore pressure, rock strength, and current mud weight to get the collapse and fracture pressure limits.

**Q: Can this tool account for shale swelling?**
Yes. The `evaluate_time_dependent_risk` tool includes an option to specify if the rock is shale, which simulates the increased degradation caused by swelling.

**Q: Does orientation affect the results?**
Yes, wellbore orientation is critical. The `calculate_collapse_pressure` tool allows you to specify if the well is vertical or deviated to ensure accurate stress concentration calculations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wellbore-stability-analysis](https://vinkius.com/en/ai-agent-connect/wellbore-stability-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wellbore Stability Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wellbore-stability-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wellbore Stability Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wellbore-stability-analysis": {
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
