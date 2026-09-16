# Wine pH Adjustment Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-ph-adjustment-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Precision tool for calculating organic acid additions to adjust wine pH and predict TA impact.

## Description
This MCP server provides enologists with precise tools to manage wine acidity. Use `calculate_acid_addition` to determine the exact mass of tartaric, malic, citric, or lactic acid needed to reach a target pH. The tool accounts for the wine's buffer capacity and volume. You can also use `predict_ph_response_curve` to visualize how different acid doses will shift the pH, or `evaluate_kbt_risk` to assess the likelihood of potassium bitartrate precipitation. For safety, `generate_trial_protocol` provides a step-by-step method for bench-top validation before bulk addition.


## Available Tools (4)
- **calculate_acid_addition**: Calculates the required mass of a specific acid to reach a target pH
- **generate_trial_protocol**: Provides a step-by-step instruction set for performing a bench-top validation of the calculation
- **predict_ph_response_curve**: Provides a series of pH values to help the user visualize how different acid doses will affect the wine
- **evaluate_kbt_risk**: Assesses the likelihood of potassium bitartrate precipitation following a planned acid addition


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine pH Adjustment Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 500L of wine with a pH of 3.6 and TA of 6.5 g/L. How much tartaric acid do I need to reach a pH of 3.4?"

**🤖 AI Agent:**
> To reach a target pH of 3.4, you need to add 142.5 grams of tartaric acid to your 500L volume. This addition is expected to increase the TA by 0.45 g/L.

---

**👤 You:**
> "Show me the pH response curve for 1000L of wine at pH 3.5 and TA 7.0 g/L using malic acid in 0.2 g/L increments."

**🤖 AI Agent:**
> The simulated pH response for malic acid addition is as follows: at 0.2 g/L the pH will be 3.46, at 0.4 g/L the pH will be 3.42, and at 0.6 g/L the pH will be 3.39.

---

**👤 You:**
> "What is the risk of KBT precipitation if I add tartaric acid to lower the pH from 3.7 to 3.4 in a wine with 250 mg/L potassium?"

**🤖 AI Agent:**
> The precipitation risk is Moderate. The estimated mass of KBT that might precipitate in a 100L volume is 12.4 grams.


## ❓ FAQ

**Q: How does this tool account for wine buffer capacity?**
The `calculate_acid_addition` tool uses a buffer capacity model that incorporates the current titratable acidity (TA) and the specific dissociation constants of the chosen acid type to ensure accurate mass calculations.

**Q: Can I check for potassium bitartrate precipitation risk?**
Yes, you can use the `evaluate_kbt_risk` tool. By providing the current pH, target pH, current TA, and potassium concentration, the tool assesses the risk of KBT precipitation.

**Q: What should I do before adding acid to a large volume of wine?**
It is highly recommended to perform a small-scale trial. You can use `generate_trial_protocol` to receive specific instructions for a bench-top validation using a concentrated stock solution.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-ph-adjustment-calculator](https://vinkius.com/en/ai-agent-connect/wine-ph-adjustment-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine pH Adjustment Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-ph-adjustment-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine pH Adjustment Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-ph-adjustment-calculator": {
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
