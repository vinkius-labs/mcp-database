# Wine Aroma Wheel Mapping MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-aroma-wheel-mapping)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Maps chemical concentrations of volatile compounds to human-perceptible wine aroma profiles.

## Description
This MCP server acts as a sensory translation engine, bridging the gap between chemical analysis and human perception. By processing volatile compound concentrations, it calculates Odor Activity Values (OAV) and applies matrix-adjusted sensory thresholds to predict how a wine will actually smell. Users can use `predict_aroma_profile` to generate a complete sensory profile, `get_dominant_categories` to identify primary aroma families, `analyze_matrix_influence` to see how alcohol and pH affect perception, and `map_to_aroma_wheel` to translate chemical data into standard Wine Aroma Wheel descriptors.


## Available Tools (4)
- **get_dominant_categories**: Identifies the high-level aroma families that define the wine
- **analyze_matrix_influence**: Evaluates how the wine's chemical environment might be masking or enhancing specific aromas
- **map_to_aroma_wheel**: Translates specific chemical intensities into standard sensory descriptors found on the Wine Aroma Wheel
- **predict_aroma_profile**: Predicts the complete sensory profile of a wine based on its chemical composition


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Aroma Wheel Mapping** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the predicted aroma profile for a wine with these concentrations: { 'isoamyl_acetate': 0.5, 'ethyl_hexyl_acetate': 0.2 }?"

**🤖 AI Agent:**
> The predicted profile includes strong notes of Banana and Pear with moderate intensity.

---

**👤 You:**
> "How will the alcohol content affect the perception of these compounds: { 'terpene_a': 0.1 } with 14% alcohol?"

**🤖 AI Agent:**
> The 14% alcohol content is expected to slightly mask the perceived intensity of the terpene concentration.

---

**👤 You:**
> "What are the dominant aroma categories for this sample: { 'methoxypyrazine': 0.05, 'linalool': 0.3 }?"

**🤖 AI Agent:**
> The dominant categories are Floral and Vegetal.


## ❓ FAQ

**Q: How does the tool account for the wine's composition?**
The server uses `analyze_matrix_influence` to evaluate how factors like alcohol content and pH levels modify the perceived intensity of specific compounds.

**Q: Can I get a full list of descriptors?**
Yes, by using `predict_aroma_profile`, you receive a detailed list of descriptors and their predicted intensities.

**Q: What is the Wine Aroma Wheel mapping?**
The `map_to_aroma_wheel` tool translates chemical data into standardized sensory categories like Fruity, Floral, or Vegetal.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-aroma-wheel-mapping](https://vinkius.com/en/ai-agent-connect/wine-aroma-wheel-mapping)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Aroma Wheel Mapping** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-aroma-wheel-mapping` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Aroma Wheel Mapping** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-aroma-wheel-mapping": {
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
