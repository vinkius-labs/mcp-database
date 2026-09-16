# Wine Polysaccharide Extraction Modeler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-polysaccharide-extraction-modeler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [food-science](../categories/food-science.md)

Predicts polysaccharide concentration, mouthfeel, and colloidal stability in wine.

## Description
This MCP server provides advanced modeling for winemaking processes. It allows AI agents to calculate polysaccharide yields (PRAGs) using `get_extraction_profile`, predict sensory characteristics like viscosity and creaminess with `predict_sensory_profile`, and evaluate wine stability via `assess_stability`. You can also use `simulate_processing_impact` to compare how different maceration or lees contact parameters affect the final wine profile.


## Available Tools (4)
- **get_extraction_profile**: Calculates the total concentration of polysaccharides (PRAGs) based on processing inputs
- **simulate_processing_impact**: Compares two different processing methods to determine the change in polysaccharide yield
- **assess_stability**: Evaluates the colloidal stability of the wine against protein precipitation
- **predict_sensory_profile**: Predicts the perceived mouthfeel properties of the wine


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Polysaccharide Extraction Modeler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the polysaccharide profile for a Chardonnay with 24 hours of skin contact and no enzyme treatment?"

**🤖 AI Agent:**
> The extraction profile for Chardonnay with 24 hours of skin contact shows a PRAG concentration of 0.45 g/L, with rhamnogalacturonan at 0.12 g/L and arabinogalactan at 0.33 g/L.

---

**👤 You:**
> "Will increasing lees contact time improve the creaminess of the wine?"

**🤖 AI Agent:**
> Increasing lees contact from 30 to 60 days is predicted to increase the creaminess score from 0.65 to 0.78 due to higher arabinogalactan release.

---

**👤 You:**
> "Is there a risk of protein precipitation for this wine?"

**🤖 AI Agent:**
> With a stability index of 0.85 and sufficient PRAG concentration, the risk of precipitation is very low.


## ❓ FAQ

**Q: How can I calculate the total polysaccharide yield?**
Use the `get_extraction_profile` tool by providing the grape variety, skin contact time, enzyme treatment status, and lees contact duration.

**Q: Can I compare two different winemaking methods?**
Yes, the `simulate_processing_impact` tool allows you to compare a base method against a target method to see changes in concentration and mouthfeel.

**Q: How is wine stability assessed?**
Stability is evaluated using `assess_stability`, which analyzes the interaction between PRAG concentrations and rhamnogalacturonan content.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-polysaccharide-extraction-modeler](https://vinkius.com/en/ai-agent-connect/wine-polysaccharide-extraction-modeler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Polysaccharide Extraction Modeler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-polysaccharide-extraction-modeler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Polysaccharide Extraction Modeler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-polysaccharide-extraction-modeler": {
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
