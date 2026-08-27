# Wine Color Extraction Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-color-extraction-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-science](../categories/data-science.md)

Models anthocyanin extraction and color stability during red wine fermentation.

## Description
This MCP server provides specialized tools for modeling the extraction kinetics of pigments during red wine fermentation. It allows winemakers and researchers to predict anthocyanin concentration using `get_anthocyanin_profile`, estimate visual depth with `predict_color_intensity`, and determine the ideal skin contact duration via `optimize_contact_duration`. Additionally, it can model the transformation of pigments using `simulate_pigment_evolution` to understand long-term color stability.


## Available Tools (4)
- **get_anthocyanin_profile**: Predicts the concentration of anthocyanins at various stages of the fermentation process
- **optimize_contact_duration**: Calculates the ideal amount of time to leave skins in contact to reach a specific target color intensity
- **predict_color_intensity**: Estimates the visual color depth of the wine based on current extraction parameters
- **simulate_pigment_evolution**: Models the transformation of simple anthocyanins into stable polymeric pigments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Color Extraction Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What will the anthocyanin concentration be for Cabernet Sauvignon after 48 hours of contact at 25°C with 13% ethanol and moderate cap management?"

**🤖 AI Agent:**
> The final anthocyanin concentration for Cabernet Sauvignon is 0.85 g/L.

---

**👤 You:**
> "How much time do I need for a Merlot to reach a color intensity of 0.7?"

**🤖 AI Agent:**
> The recommended contact time to reach a target intensity of 0.7 for Merlot is 72 hours.

---

**👤 You:**
> "Predict the color stability for a wine with 0.9 anthocyanin concentration and 0.4 polymeric pigment level at 14% ethanol."

**🤖 AI Agent:**
> The predicted color stability index is 0.78.


## ❓ FAQ

**Q: How can I predict the final color of my wine?**
You can use `predict_color_intensity` after obtaining the concentration data from `get_anthocyanin_profile` to estimate the visual depth and stability.

**Q: Can I optimize skin contact time?**
Yes, the `optimize_contact_duration` tool calculates the minimum time required to reach your specific target color intensity based on grape variety and fermentation conditions.

**Q: Does temperature affect the results?**
Yes, temperature is a key input for `get_anthocyanin_profile` and `optimize_contact_duration` as it directly influences the diffusion kinetics of pigment extraction.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-color-extraction-model](https://vinkius.com/ai-agent-connect/wine-color-extraction-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Color Extraction Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-color-extraction-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Color Extraction Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-color-extraction-model": {
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
