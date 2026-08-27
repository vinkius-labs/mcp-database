# Wine Aging Kinetics Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-aging-kinetics-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Predict wine color, astringency, and aroma evolution using chemical kinetics.

## Description
This MCP server provides advanced chemical kinetics modeling to predict how wine evolves during the aging process. By analyzing initial phenolic composition and environmental factors like oxygen exposure and temperature, the server calculates critical aging trajectories. Use `get_color_evolution` to predict hue and intensity shifts, `get_astringency_profile` to estimate mouthfeel changes, `get_aroma_trajectory` to forecast the transition from primary fruit to tertiary aromas, and `get_aging_regime` to identify if the wine is following an oxidative or reductive path.


## Available Tools (4)
- **get_aroma_trajectory**: Predicts the shift from primary fruit aromas to tertiary aged aromas
- **get_astringency_profile**: Estimates the perceived mouthfeel and structural tightness of the wine
- **get_color_evolution**: Predicts the visual changes in wine color based on chemical shifts
- **get_aging_regime**: Determines if the wine is undergoing oxidative or reductive aging


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Aging Kinetics Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What will the color of this wine look like after 5 years at 15°C with high anthocyanin levels?"

**🤖 AI Agent:**
> The wine is predicted to shift toward a Garnet hue with a color intensity of 0.65.

---

**👤 You:**
> "How much astringency will remain after 10 years of aging?"

**🤖 AI Agent:**
> The predicted astringency score is 0.25, indicating a significant reduction in perceived puckering due to tannin polymerization.

---

**👤 You:**
> "Will this wine develop leather aromas if exposed to 5 mg/L of oxygen over 3 years?"

**🤖 AI Agent:**
> Yes, the wine is predicted to show a strong presence of Leather as a tertiary aroma profile.


## ❓ FAQ

**Q: How does temperature affect the predictions?**
Temperature acts as a kinetic driver; higher temperatures accelerate the reaction rates of anthocyanin-tannin polymerization, leading to faster color and astringency changes.

**Q: Can I predict the specific aroma profile of an aged wine?**
Yes, by using `get_aroma_trajectory`, you can predict the dominant tertiary aroma profiles, such as Vanilla or Leather, based on oxygen exposure and duration.

**Q: What is the difference between oxidative and reductive regimes?**
The `get_aging_regime` tool classifies the process based on oxygen availability. Oxidative regimes involve higher oxygen exposure, while reductive regimes occur in low-oxygen environments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-aging-kinetics-predictor](https://vinkius.com/ai-agent-connect/wine-aging-kinetics-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Aging Kinetics Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-aging-kinetics-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Aging Kinetics Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-aging-kinetics-predictor": {
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
