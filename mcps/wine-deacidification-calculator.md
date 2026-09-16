# Wine Deacidification Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-deacidification-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Precision tools for calculating deacidification dosage and stability risks in wine.

## Description
This MCP server provides enologists with precise chemical calculation tools to manage wine acidity. Use `calculate_reagent_dosage` to determine the exact mass of calcium carbonate, potassium bicarbonate, or double salt needed to reach a target TA. Assess the likelihood of crystal formation using `evaluate_stability_risk` based on pH and acid ratios. For early-stage management, `simulate_prefermentation_treatment` models the impact of double salts on malic acid levels, while `get_acid_profile` provides a detailed breakdown of acid composition.


## Available Tools (4)
- **calculate_reagent_dosage**: Determines the exact mass of a specific deacidifying agent required to reach a desired acidity level
- **get_acid_profile**: Provides a summary of the acid composition and calculates the specific acid ratio
- **simulate_prefermentation_treatment**: Models the effects of using double salts during the prefermentation stage
- **evaluate_stability_risk**: Consider current pH and the malic-to-tartaric acid ratio.

Predicts the likelihood of tartrate precipitation following a deacidification treatment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Deacidification Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much calcium carbonate do I need for 500L of wine with 7.5 g/L TA to reach 5.0 g/L?"

**🤖 AI Agent:**
> To reach a target TA of 5.0 g/L in 500L of wine, you need to add 1250 grams of calcium carbonate.

---

**👤 You:**
> "What is the stability risk for a wine with pH 3.2, TA 6.0, and a malic-to-tartaric ratio of 0.5 after reducing TA to 4.5?"

**🤖 AI Agent:**
> The stability risk is Moderate. Reducing the TA to 4.5 g/L at a pH of 3.2 increases the likelihood of tartrate precipitation.

---

**👤 You:**
> "Calculate the acid profile for a wine with 5.0 g/L tartaric acid and 2.0 g/L malic acid."

**🤖 AI Agent:**
> The total acid concentration is 7.0 g/L, and the malic-to-tartaric acid ratio is 0.4.


## ❓ FAQ

**Q: How do I calculate the amount of reagent needed?**
You can use the `calculate_reagent_dosage` tool by providing the current TA, target TA, and the total wine volume.

**Q: Can I predict if my wine will precipitate crystals?**
Yes, the `evaluate_stability_risk` tool predicts the likelihood of tartrate precipitation based on your current pH and acid ratio.

**Q: What is the difference between the treatment types?**
The tools support calcium carbonate, potassium bicarbonate, and double salt, each with different stoichiometric impacts on pH and TA.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-deacidification-calculator](https://vinkius.com/en/ai-agent-connect/wine-deacidification-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Deacidification Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-deacidification-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Deacidification Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-deacidification-calculator": {
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
