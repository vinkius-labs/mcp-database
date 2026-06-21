# Hydration Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hydration-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [baking](../categories/baking.md)

Predict dough texture and hydration percentage instantly for bread, pizza, or focaccia.

## Description
**Are you guessing your dough's final structure?** Hydration is the single most critical factor in baking success. Too dry, and your bread won't rise; too wet, and it will collapse. Getting this ratio right--especially when adding non-water liquids like oil or eggs--is difficult for even experienced bakers.


## Available Tools
- **calculate_hydration**: Use this to determine how wet or dry a dough mixture is.

Calculate dough hydration percentage from flour and liquid weights
- **classify_texture**: Classify dough texture from hydration percentage and profile name
- **determine_dough_type**: Helps identify what kind of baked good the ingredients are suited for.

Determine dough type from flour and salt composition


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hydration Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 100g of '00' flour, 75g of water, and 20g of olive oil. Can you calculate the hydration and predict the texture for a pizza?"

**🤖 AI Agent:**
> First, using `calculate_hydration`, I found your effective liquid weight is 95g (75g water + 20g oil), giving you a hydration of [CALCULATED_HYDRATION]%. Next, running `determine_dough_type` confirmed this as 'Neapolitan Pizza Crust'. Finally, the `classify_texture` tool predicts your texture will be [PREDICTED_TEXTURE], with suitability notes: [SUITABILITY_NOTES].

---

**👤 You:**
> "I'm making a rustic loaf. I used 450g of bread flour, 20g of salt, and 350g of water. What is the best texture profile?"

**🤖 AI Agent:**
> Based on your ingredients (Bread Flour, 450g flour / 20g salt), `determine_dough_type` suggests a 'Rustic European Loaf' profile. The hydration calculated by `calculate_hydration` is [CALCULATED_HYDRATION]%. Therefore, the final classification from `classify_texture` is [PREDICTED_TEXTURE], suggesting you need to focus on [SUITABILITY_NOTES].

---

**👤 You:**
> "I have a high hydration dough (85%) and confirmed the profile is Chapati. What should I expect?"

**🤖 AI Agent:**
> Running `classify_texture` with 85% hydration and 'Chapati' profile, we get a result of [PREDICTED_TEXTURE] classification. The suitability notes advise that [SUITABILITY_NOTES]. This confirms the specific constraints needed for flatbreads.


## ❓ FAQ

**Q: How is dough hydration calculated?**
You use the `calculate_hydration` tool. This function takes your total flour weight, total water weight, and any liquid additives (like oil or milk) to give you a precise percentage of hydration.

**Q: What if I don't know my dough type?**
Before calculating texture, run the `determine_dough_type` tool. By providing your flour type and salt weight, this tool establishes a structural profile (e.g., Neapolitan Pizza) that provides necessary context for accurate prediction.

**Q: Does the texture classification rely on multiple inputs?**
Yes. The `classify_texture` tool is designed to take two specific pieces of information: 1) your calculated hydration percentage, and 2) the confirmed dough profile name provided by the `determine_dough_type` tool. Both are required for an accurate result.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hydration-calculator](https://vinkius.com/mcp/hydration-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hydration Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `hydration-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hydration Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hydration-calculator": {
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
