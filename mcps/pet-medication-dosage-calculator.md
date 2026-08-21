# Pet Medication Dosage Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/pet-medication-dosage-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Deterministic pet medication dosage calculator with species-specific safety checks.

## Description
This MCP server provides precise medication administration calculations for pets. It handles species-specific safety thresholds for dogs and cats, automatically adjusts for pediatric and geriatric life stages, and converts weight between kg and lbs. Use `calculate_single_dose` to find individual administration amounts, `calculate_daily_requirements` for 24-hour totals, and `get_syringe_markings` to assist with liquid dosing accuracy.


## Available Tools (3)
- **get_syringe_markings**: Provides the volume per individual marking on a syringe for liquid medication
- **calculate_daily_requirements**: Calculates the total amount of medication required for a full 24-hour period
- **calculate_single_dose**: Determines the specific amount of medication to be given in a single administration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Medication Dosage Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a single dose for a 5kg dog receiving 10mg/kg of liquid medication, given twice daily."

**🤖 AI Agent:**
> The dose for this dog is 2.5 ml per administration.

---

**👤 You:**
> "What is the total daily requirement for a 15lb cat taking 5mg/kg of a tablet medication, once daily?"

**🤖 AI Agent:**
> The total daily requirement is 0.34 tablets.

---

**👤 You:**
> "I have a 3ml syringe. How much volume does each marking represent for a 1.5ml dose?"

**🤖 AI Agent:**
> Each marking on the syringe represents 0.1 ml.


## ❓ FAQ

**Q: How does the calculator handle different animal ages?**
The calculator applies specific multipliers for pediatric animals (under 6 months) and geriatric animals (over 10 years) to ensure dosage rates remain within safe physiological limits.

**Q: Can I use this for both liquid and tablet medications?**
Yes. By using `calculate_single_dose`, you can specify if the medication is liquid (returning ml) or a tablet (returning pill count).

**Q: What happens if a dosage is too high?**
The `calculate_single_dose` tool compares the prescribed rate against species-specific safety thresholds. If the rate is too high, it flags the dose as dangerous and provides a warning message.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/pet-medication-dosage-calculator](https://vinkius.com/ai-agent-connect/pet-medication-dosage-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Medication Dosage Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-medication-dosage-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Medication Dosage Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-medication-dosage-calculator": {
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
