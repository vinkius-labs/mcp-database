# Wine MLF Optimization Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-mlf-optimization-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [optimization](../categories/optimization.md)

Optimize Malolactic Fermentation timing, dosage, and nutrient needs.

## Description
This MCP server provides specialized tools for winemakers to manage Malolactic Fermentation (MLF). It calculates the ideal timing using `calculate_inoculation_strategy`, determines the required bacterial dosage with `determine_inoculation_rate`, identifies necessary nutrient support via `estimate_nutrient_needs`, and predicts the completion timeline using `predict_mlf_duration`. The engine accounts for environmental stressors like alcohol, pH, and SO2 to ensure bacterial viability.


## Available Tools (4)
- **predict_mlf_duration**: Predicts how long the malolactic fermentation process will take to complete
- **calculate_inoculation_strategy**: Determines whether to use co-inoculation or sequential inoculation based on environmental stressors
- **determine_inoculation_rate**: Calculates the necessary amount of bacterial culture to add to the wine
- **estimate_nutrient_needs**: Identifies if and how much supplemental nutrients are needed to support the bacteria


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine MLF Optimization Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Should I use co-inoculation or sequential inoculation for a wine with 13% alcohol, pH 3.2, and 30 mg/L SO2?"

**🤖 AI Agent:**
> The recommended strategy is sequential inoculation due to the high stress score from the alcohol and SO2 levels.

---

**👤 You:**
> "How many days will MLF take if I have 2.0 g/L malic acid, a temperature of 20°C, and a dosage of 50 g/hL?"

**🤖 AI Agent:**
> The estimated duration for malic acid conversion is 12 days.

---

**👤 You:**
> "What nutrients are needed for a wine with 4.0 g/L malic acid and a stress score of 0.8?"

**🤖 AI Agent:**
> The required nutrient profile is high, with a suggested supplemental amount of 15.5 g/hL.


## ❓ FAQ

**Q: How do I decide between co-inoculation and sequential inoculation?**
Use the `calculate_inoculation_strategy` tool. It analyzes alcohol, pH, and SO2 levels to determine if the environment is too hostile for early inoculation.

**Q: Can I predict how long my MLF will take?**
Yes, the `predict_mlf_duration` tool estimates the number of days until malic acid conversion is complete based on temperature and dosage.

**Q: What factors influence the required bacterial dosage?**
The `determine_inoculation_rate` tool calculates dosage by considering the chosen strategy and environmental stressors like alcohol and SO2.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-mlf-optimization-engine](https://vinkius.com/en/ai-agent-connect/wine-mlf-optimization-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine MLF Optimization Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-mlf-optimization-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine MLF Optimization Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-mlf-optimization-engine": {
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
