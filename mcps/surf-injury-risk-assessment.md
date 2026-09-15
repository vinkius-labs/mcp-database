# Surf Injury Risk Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/surf-injury-risk-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [safety](../categories/safety.md)

Evaluates physical injury risk for surfers based on ocean conditions, gear, and fatigue.

## Description
This MCP server provides critical safety analysis for surfers. By connecting to Vinkius Edge, AI agents can use `calculate_risk_profile` to assess overall danger, `evaluate_equipment_safety` to verify gear suitability, `check_fatigue_impact` to quantify exhaustion risks, and `get_environmental_threat_level` to identify oceanographic hazards like rip currents. It helps surfers make informed decisions about when to enter the water and what equipment to use.


## Available Tools (4)
- **calculate_risk_profile**: Provides a comprehensive assessment of the current injury risk for a specific surfer in specific conditions
- **check_fatigue_impact**: Quantifies how much the surfer's current exhaustion level is amplifying the existing environmental risks
- **evaluate_equipment_safety**: Determines if the chosen gear is appropriate for the current sea state
- **get_environmental_threat_level**: Analyzes wave and wind patterns to identify specific oceanographic dangers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surf Injury Risk Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my injury risk for 5ft waves, 10s swell, offshore wind, using a longboard, as an intermediate surfer with low fatigue?"

**🤖 AI Agent:**
> Your risk level is Low. The conditions are manageable for your skill level and equipment.

---

**👤 You:**
> "Is my shortboard safe for 8ft waves in 20°C water?"

**🤖 AI Agent:**
> No, the gear is not appropriate. A shortboard may be difficult to control in 8ft waves; a larger board is suggested.

---

**👤 You:**
> "I am feeling high fatigue. How much does this increase my risk if my base score was 40?"

**🤖 AI Agent:**
> Your amplified risk score is 120, and you have entered the danger zone due to high fatigue.


## ❓ FAQ

**Q: How does the tool account for physical exhaustion?**
The tool uses `check_fatigue_impact` to calculate how much a surfer's exhaustion level increases their base risk score, potentially pushing them into a danger zone.

**Q: Can I check if my surfboard is safe for large waves?**
Yes, you can use `evaluate_equipment_safety` to determine if your specific gear is appropriate for the current wave size and water temperature.

**Q: What kind of ocean threats can be identified?**
By using `get_environmental_threat_level`, the tool identifies primary threats such as Rip Currents, Heavy Impact, or high turbulence based on swell and wind.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/surf-injury-risk-assessment](https://vinkius.com/en/ai-agent-connect/surf-injury-risk-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surf Injury Risk Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surf-injury-risk-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surf Injury Risk Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surf-injury-risk-assessment": {
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
