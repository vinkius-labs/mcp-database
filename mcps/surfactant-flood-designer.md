# Surfactant Flood Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/surfactant-flood-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [energy](../categories/energy.md)

Designs surfactant floods for Enhanced Oil Recovery (EOR) by modeling phase behavior and IFT reduction.

## Description
This MCP server provides specialized tools for designing surfactant flooding operations in Enhanced Oil Recovery (EOR). It enables AI agents to calculate optimal surfactant types, determine required salinity and co-solvent concentrations for ultra-low IFT, design injection slugs accounting for adsorption, and predict incremental oil recovery. By using `get_optimal_surfactant_type`, `calculate_phase_parameters`, `design_injection_slug`, and `estimate_oil_recovery`, users can model complex reservoir interactions and chemical front behaviors.


## Available Tools (4)
- **calculate_phase_parameters**: Determines the required salinity and co-solvent amount to achieve ultra-low IFT
- **design_injection_slug**: Calculates the technical specifications for the surfactant injection volume and concentration
- **estimate_oil_recovery**: Predicts the incremental oil recovery percentage resulting from the surfactant flood
- **get_optimal_surfactant_type**: Recommends the most effective surfactant class based on oil properties and reservoir conditions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surfactant Flood Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the best surfactant for a high asphaltene oil at 80 degrees Celsius and 3000 psi?"

**🤖 AI Agent:**
> The recommended surfactant category for high asphaltene oil at these conditions is Anionic.

---

**👤 You:**
> "Calculate the required salinity and co-solvent for an anionic surfactant in paraffinic oil to reach a target IFT of 0.001."

**🤖 AI Agent:**
> The optimal salinity is 15000 ppm and the required co-solvent concentration is 5% of the total volume.

---

**👤 You:**
> "Estimate the oil recovery for an initial saturation of 0.7, a capillary number of 1e-3, and a slug size of 0.5 pore volumes."

**🤖 AI Agent:**
> The predicted incremental oil recovery is 12.5% with an expected residual oil saturation of 0.575.


## ❓ FAQ

**Q: How does this tool help with EOR design?**
It automates the calculation of critical parameters like optimal salinity and slug size using `calculate_phase_parameters` and `design_injection_slug` to ensure effective oil mobilization.

**Q: Can I predict oil recovery percentages?**
Yes, the `estimate_oil_recovery` tool predicts incremental oil recovery based on the capillary number and the designed slug size.

**Q: Does it account for surfactant loss?**
Yes, the `design_injection_slug` tool specifically incorporates the adsorption rate to calculate the effective concentration remaining in the reservoir.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/surfactant-flood-designer](https://vinkius.com/en/ai-agent-connect/surfactant-flood-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surfactant Flood Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surfactant-flood-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surfactant Flood Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surfactant-flood-designer": {
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
