# Quantitative Risk Assessment (QRA) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/quantitative-risk-assessment-qra)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Perform safety and environmental impact modeling for oil and gas facilities.

## Description
This MCP server provides specialized analytical tools for Quantitative Risk Assessment (QRA) in high-consequence environments like oil and gas facilities. It allows AI agents to calculate critical safety metrics including adjusted hazard frequencies, individual risk, and societal risk. Users can model the impact of hazardous events and generate data for FN curves to visualize cumulative fatality risks. Key tools include `analyze_hazard_frequency` for statistical likelihood, `calculate_individual_risk` for proximity-based assessment, `evaluate_societal_risk` for population impact, and `generate_fn_curve_data` for graphical risk modeling.


## Available Tools (4)
- **analyze_hazard_frequency**: Determines the statistical likelihood of identified hazards
- **calculate_individual_risk**: Estimates the risk to a specific individual based on proximity to hazards
- **evaluate_societal_risk**: Estimates the risk to a population for a specific event
- **generate_fn_curve_data**: Produces the data points required to plot an FN curve for societal risk


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Quantitative Risk Assessment (QRA)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the adjusted frequency for hazard 'tank_rupture' if the base frequency is 0.01 and the mitigation factor is 0.5?"

**🤖 AI Agent:**
> The adjusted frequency for the tank rupture hazard is 0.005.

---

**👤 You:**
> "Calculate the individual risk for a hazard with frequency 0.02, vulnerability 1.5, and consequence severity 10."

**🤖 AI Agent:**
> The calculated individual risk is 0.3.

---

**👤 You:**
> "Evaluate the societal risk for an event with frequency 0.05, a population of 200, and a vulnerability factor of 1.2."

**🤖 AI Agent:**
> The expected fatalities are 240 and the total societal risk is 12.


## ❓ FAQ

**Q: What can I calculate with this server?**
You can use `analyze_hazard_frequency` to find adjusted hazard probabilities, `calculate_individual_risk` for person-specific risk, and `evaluate_societal_risk` to determine the impact on larger populations.

**Q: How do I model mitigation measures?**
Use the `analyze_hazard_frequency` tool and provide `mitigationFactors` to reduce the baseline frequency of identified hazards.

**Q: Can I generate FN curves?**
Yes, the `generate_fn_curve_data` tool produces the necessary data points for plotting cumulative frequency against fatality counts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/quantitative-risk-assessment-qra](https://vinkius.com/en/ai-agent-connect/quantitative-risk-assessment-qra)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Quantitative Risk Assessment (QRA)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `quantitative-risk-assessment-qra` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Quantitative Risk Assessment (QRA)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "quantitative-risk-assessment-qra": {
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
