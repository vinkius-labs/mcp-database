# Blast Fragmentation Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/blast-fragmentation-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Predict rock fragmentation size distributions using the Kuz-Ram model.

## Description
This MCP server provides predictive modeling for mining operations to calculate rock fragmentation size distributions. By integrating rock mass characteristics, blast pattern parameters, and explosive energy, it uses the Kuz-Ram model to provide critical metrics. Use `predict_fragmentation_distribution` to calculate P50 and P80 sizes, `evaluate_pattern_efficiency` to analyze muckpile uniformity, `calculate_oversize_risk` to assess boulder production, and `simulate_energy_impact` to predict how energy adjustments shift the distribution.


## Available Tools (4)
- **calculate_oversize_risk**: Specifically assesses the likelihood of producing "boulders" that exceed operational limits
- **evaluate_pattern_efficiency**: Analyzes how different blast patterns affect the uniformity of the resulting muckpile
- **predict_fragmentation_distribution**: Calculates the primary fragmentation statistics for a specific blast design
- **simulate_energy_impact**: Predicts how changing the explosive energy or specific charge will shift the fragmentation distribution


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blast Fragmentation Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the fragmentation distribution for a rock with factor 10, burden 3, spacing 4, diameter 0.15, specific charge 0.5, and explosive energy 1.0."

**🤖 AI Agent:**
> The predicted median size (P50) is 12.4 cm, the P80 is 25.8 cm, the uniformity index is 1.15, and the oversize percentage is 4.2%.

---

**👤 You:**
> "What is the risk of oversize if my P80 is 35cm and my maximum allowable size is 30cm with a rock factor of 12?"

**🤖 AI Agent:**
> The calculated oversize probability is 28% and the risk level is Medium.

---

**👤 You:**
> "How will increasing explosive energy by 20% affect my fragmentation?"

**🤖 AI Agent:**
> Increasing the energy by 20% is predicted to reduce the P50 from 15.0 cm to 13.2 cm, representing a 12% improvement in median size.


## ❓ FAQ

**Q: What is the Kuz-Ram model?**
The Kuz-Ram model is a mathematical framework used to predict the size distribution of rock fragments resulting from blasting operations.

**Q: How can I check if my blast pattern will produce too many large rocks?**
You can use the `calculate_oversize_risk` tool to assess the likelihood of producing boulders that exceed your specific operational limits.

**Q: Can I simulate changes in explosive energy?**
Yes, the `simulate_energy_impact` tool allows you to predict how adjusting the explosive energy or specific charge will shift the fragmentation distribution.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/blast-fragmentation-model](https://vinkius.com/ai-agent-connect/blast-fragmentation-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Blast Fragmentation Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `blast-fragmentation-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Blast Fragmentation Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blast-fragmentation-model": {
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
