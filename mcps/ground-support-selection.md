# Ground Support Selection MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ground-support-selection)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Specialized decision-support for geotechnical excavation stability.

## Description
This MCP server provides specialized geotechnical engineering tools to ensure excavation stability in mining and civil tunneling. It allows AI agents to calculate specific physical support components, assess safety margins, and determine corrosion mitigation strategies based on rock mass conditions, excavation span, and service life. Use `calculate_support_requirements` to determine bolt patterns and shotcrete thickness, `evaluate_stability_safety_margin` to check stability status, and `get_corrosion_mitigation_strategy` for long-term protection recommendations.


## Available Tools (4)
- **compare_support_options**: Compares two different support configurations to aid in cost-benefit or safety-benefit analysis
- **evaluate_stability_safety_margin**: Assesses how much additional load the selected support can handle before failure
- **get_corrosion_mitigation_strategy**: Provides specific technical recommendations for protecting support elements based on the environment
- **calculate_support_requirements**: Determines the specific physical support components needed for a given excavation scenario


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ground Support Selection** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What support is needed for a 5 meter span in poor rock mass with a 10 year service life?"

**🤖 AI Agent:**
> For a 5 meter span in poor rock mass with a 10 year service life, the recommended support is Rock Bolts with a pattern of 1.2m spacing and 15cm of shotcrete.

---

**👤 You:**
> "Is my current support stable for a 12 meter span in fair rock?"

**🤖 AI Agent:**
> The stability status for a 12 meter span in fair rock with the selected support is stable, with a safety factor of 1.65.

---

**👤 You:**
> "What corrosion protection should I use for a 50 year service life in a seismic zone?"

**🤖 AI Agent:**
> For a 50 year service life in a seismic zone, the recommended mitigation method is epoxy_coated reinforcement with a maintenance interval of 24 months.


## ❓ FAQ

**Q: How do I determine the required shotcrete thickness?**
You can use the `calculate_support_requirements` tool, providing the rock mass condition, excavation span, and service life to receive the exact thickness required.

**Q: Can this tool account for seismic activity?**
Yes, by setting the `isSeismicZone` parameter to true in `calculate_support_requirements`, the system will prioritize energy-absorbing reinforcement.

**Q: How is the safety factor calculated?**
The safety factor is calculated using `evaluate_stability_safety_margin`, which analyzes the relationship between rock strength and applied stress from the span.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ground-support-selection](https://vinkius.com/ai-agent-connect/ground-support-selection)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ground Support Selection** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ground-support-selection` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ground Support Selection** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ground-support-selection": {
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
