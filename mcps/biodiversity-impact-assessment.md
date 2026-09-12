# Biodiversity Impact Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/biodiversity-impact-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environment](../categories/environment.md)

Assess ecological impacts from industrial operations using habitat and species data.

## Description
This MCP server provides specialized tools to evaluate the biological consequences of industrial projects, such as oil and gas operations. It allows users to calculate total habitat loss via `get_habitat_loss_summary`, evaluate connectivity risks using `assess_fragmentation_risk`, and measure biological consequences through `evaluate_species_impact`. Additionally, it ensures environmental compliance by using `audit_mitigation_hierarchy` to verify that mitigation plans follow the mandatory avoidance, minimization, restoration, and offsetting sequence.


## Available Tools (4)
- **audit_mitigation_hierarchy**: Checks if a proposed mitigation plan adequately follows the mandatory priority sequence
- **evaluate_species_impact**: Measures the biological consequence of project activities based on the presence of sensitive species
- **get_habitat_loss_summary**: Calculates the total amount of habitat lost across all types within a project footprint
- **assess_fragmentation_risk**: Evaluates the risk that industrial infrastructure will split large habitats into smaller, disconnected pieces


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Biodiversity Impact Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the habitat loss for a 500 hectare project where 50 hectares of rainforest and 20 hectares of grassland are impacted."

**🤖 AI Agent:**
> The total area lost is 70 hectares, consisting of 50 hectares of rainforest and 20 hectares of grassland.

---

**👤 You:**
> "What is the fragmentation risk for a 100km pipeline passing through a habitat that is 5km wide?"

**🤖 AI Agent:**
> The fragmentation index is high due to the significant length of the pipeline relative to the habitat width, creating a substantial edge effect area.

---

**👤 You:**
> "Is a mitigation plan that only uses offsetting compliant with the hierarchy?"

**🤖 AI Agent:**
> No, the plan is non-compliant because it fails to address avoidance and minimization before moving to offsetting.


## ❓ FAQ

**Q: How do I calculate the total area of habitat lost?**
You can use the `get_habitat_loss_summary` tool by providing the total project footprint area and a map of the impacted habitat types.

**Q: Can this tool check if my mitigation plan is valid?**
Yes, the `audit_mitigation_hierarchy` tool checks if your proposed actions follow the required priority sequence of avoidance, minimization, restoration, and offsetting.

**Q: How is species risk calculated?**
The `evaluate_species_impact` tool calculates risk by weighting the presence of species against their IUCN Red List categories and the magnitude of habitat loss.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/biodiversity-impact-assessment](https://vinkius.com/en/ai-agent-connect/biodiversity-impact-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Biodiversity Impact Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `biodiversity-impact-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Biodiversity Impact Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "biodiversity-impact-assessment": {
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
