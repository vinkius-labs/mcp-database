# Wine Reductive Compound Formation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-reductive-compound-formation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Predictive modeling for reductive sulfur compound formation in wine.

## Description
This MCP server provides predictive modeling for assessing the risk of reductive sulfur compound formation during wine maturation. It uses sulfur compound formation kinetics to calculate predicted H2S, mercaptan, and disulfide levels. By analyzing yeast lees contact time, oxidation-reduction potential, copper residues, and nutrient status, the server can determine sensory threshold exceedance risks. Use `get_sulfur_prediction` to model concentrations, `assess_sensory_risk` to evaluate detection limits, `calculate_remediation_window` for actionable timing, and `get_autolysis_impact` to estimate yeast cell breakdown contributions.


## Available Tools (4)
- **calculate_remediation_window**: Provides actionable timing for corrective cellar operations
- **get_autolysis_impact**: Estimates the contribution of yeast cell breakdown to the total sulfur precursor pool
- **get_sulfur_prediction**: Predicts the concentration of specific reductive compounds based on current wine conditions
- **assess_sensory_risk**: Determines if the predicted sulfur concentrations will exceed human detection limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Reductive Compound Formation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Predict the sulfur compounds for a wine with 30 days of lees contact, an ORP of -150mV, 50ppb copper, and a nutrient score of 0.8."

**🤖 AI Agent:**
> The predicted concentrations are H2S: 12ppb, Mercaptan: 5ppb, and Disulfide: 8ppb.

---

**👤 You:**
> "Is there a sensory risk for a wine with the following prediction: {"h2sConcentration": 45, "mercaptanConcentration": 10, "disulfideConcentration": 5}?"

**🤖 AI Agent:**
> The risk level is High, with a high probability of threshold exceedance for H2S.

---

**👤 You:**
> "What is the impact of autolysis for 45 days of lees contact and a nutrient score of 0.4?"

**🤖 AI Agent:**
> The current precursor load is 25ppb with a precursor release rate of 0.5ppb per day.


## ❓ FAQ

**Q: How do I predict sulfur levels in my wine?**
You can use the `get_sulfur_prediction` tool by providing the yeast lees contact time, ORP, copper residue level, and nutrient status score.

**Q: Can this tool help with cellar management?**
Yes, by using `calculate_remediation_window`, you can receive actionable timing for corrective cellar operations based on predicted risks.

**Q: What factors influence the sulfur prediction?**
The prediction accounts for yeast lees contact time, oxidation-reduction potential, copper residues, and nutrient status, including the impact of autolysis.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-reductive-compound-formation](https://vinkius.com/en/ai-agent-connect/wine-reductive-compound-formation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Reductive Compound Formation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-reductive-compound-formation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Reductive Compound Formation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-reductive-compound-formation": {
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
