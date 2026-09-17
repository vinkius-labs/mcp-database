# Wine Oxidative Polymerization Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-oxidative-polymerization-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Predictive chemical modeling of phenolic polymerization and wine oxidation.

## Description
This MCP server provides a predictive engine for modeling the chemical transformation of phenolic compounds during wine oxidation. It allows AI agents to calculate polymeric pigment formation, predict color shifts (hue changes), and assess the evolution of mouthfeel and astringency. By analyzing the interaction between anthocyanins and tannins, the model accounts for oxygen exposure, acetaldehyde levels, and the inhibitory effects of glutathione. Use `predict_pigment_formation` to model pigment mass, `calculate_color_evolution` to track hue changes, `assess_sensory_impact` to monitor astringency, and `evaluate_browning_risk` to identify excessive oxidation risks.

### Available Tools

`predict_pigment_formation_tool`, `calculate_color_evolution_tool`, `assess_sensory_impact_tool`, `evaluate_browning_risk_tool`


## Available Tools (4)
- **calculate_color_evolution_tool**: g., from ruby to brick or brown) based on the mass of polymeric pigments and time elapsed.

Predicts how the visual appearance (hue) of the wine will change over a specific duration
- **evaluate_browning_risk_tool**: Provides a high-level risk assessment of whether the wine is undergoing excessive, undesirable oxidation
- **predict_pigment_formation_tool**: Calculates the expected increase in polymeric pigments based on current chemical concentrations and oxygen exposure
- **assess_sensory_impact_tool**: Predicts the evolution of mouthfeel, specifically the change in astringency


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Oxidative Polymerization Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the pigment formation for a wine with 0.5 anthocyanin, 0.8 tannin, 10 oxygen exposure, and 0.2 acetaldehyde."

**🤖 AI Agent:**
> The expected polymeric pigment mass is 0.12 units with a stability index of 0.85.

---

**👤 You:**
> "What will be the color of a ruby wine after 100 days of oxidation if the pigment mass is 0.5?"

**🤖 AI Agent:**
> The predicted hue is brick red with moderate color saturation.

---

**👤 You:**
> "Assess the sensory impact for a wine starting at 0.7 astringency with 0.4 tannin concentration and 0.2 pigment mass."

**🤖 AI Agent:**
> The current astringency is 0.55, resulting in increased mouthfeel smoothness.


## ❓ FAQ

**Q: How does this model handle antioxidant effects?**
The model accounts for glutathione competition, which reduces the effective rate of polymerization by consuming reactive quinones. Tools available: `predict_pigment_formation_tool`, `calculate_color_evolution_tool`, `assess_sensory_impact_tool`.

**Q: Can I predict the color change of my wine?**
Yes, by using `calculate_color_evolution` with the calculated polymeric pigment mass and the duration of oxidation.

**Q: What determines the browning risk?**
Browning risk is primarily driven by high oxygen exposure and acetaldehyde levels, especially when glutathione levels are low.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-oxidative-polymerization-model](https://vinkius.com/en/ai-agent-connect/wine-oxidative-polymerization-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Oxidative Polymerization Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-oxidative-polymerization-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Oxidative Polymerization Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-oxidative-polymerization-model": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
