# Wine Nutrient Addition Timing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-nutrient-addition-timing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Optimize nutrient timing to maximize aroma and prevent yeast stress.

## Description
This MCP server provides specialized tools for managing yeast health during fermentation. By monitoring Yeast Assimilable Nitrogen (YAN) and stress indicators, users can use `calculate_addition_schedule` to determine precise nutrient doses and timing. The server also includes `evaluate_aroma_potential` to predict aromatic quality and `simulate_nutrient_impact` to test additions before they are applied. It helps winemakers prevent stuck fermentations and optimize the production of esters and thiols.


## Available Tools (4)
- **simulate_nutrient_impact**: Allows the user to test a specific nutrient addition before applying it to the real fermentation
- **calculate_addition_schedule**: Determines when to add nutrients and in what quantities to maintain optimal yeast health and aroma production
- **evaluate_aroma_potential**: Predicts how the current nutrient profile will affect the wine's aromatic profile
- **get_current_status**: Provides a snapshot of the current fermentation health relative to nutrient needs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Nutrient Addition Timing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My initial YAN was 150 mg/L, current YAN is 80 mg/L, and I am at the mid-ferment stage with a stress level of 0.4. What should I do?"

**🤖 AI Agent:**
> Based on your current status, you should add 25 g/hL of organic nitrogen at the mid-ferment stage to stabilize the yeast and maintain aroma potential.

---

**👤 You:**
> "What happens if I add 10 g/hL of DAP when my current YAN is 50 mg/L and stress is 0.2?"

**🤖 AI Agent:**
> Adding 10 g/hL of DAP will increase your YAN to 60 mg/L and is expected to reduce your stress level by 0.1.

---

**👤 You:**
> "Check my current fermentation health. Initial YAN 200, current 120, stress 0.1."

**🤖 AI Agent:**
> Your current status is Optimal. The nitrogen deficit is 80 mg/L relative to your starting point.


## ❓ FAQ

**Q: How do I know if my yeast is stressed?**
You can use `get_current_status` to receive a summary of yeast vigor and identify if the current state is Optimal, Stressed, or Critical.

**Q: Can I test a nutrient addition before performing it?**
Yes, the `simulate_nutrient_impact` tool allows you to predict the new YAN level and the expected reduction in stress before you commit to an addition.

**Q: How does this help with wine aroma?**
By using `evaluate_aroma_potential`, you can predict how your nitrogen profile affects aromatic quality, helping to maximize the production of varietal-defining compounds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-nutrient-addition-timing](https://vinkius.com/en/ai-agent-connect/wine-nutrient-addition-timing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Nutrient Addition Timing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-nutrient-addition-timing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Nutrient Addition Timing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-nutrient-addition-timing": {
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
