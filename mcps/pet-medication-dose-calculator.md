# Pet Medication Dose Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pet-medication-dose-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Calculate estimated medication dosages for pets based on body weight and veterinary standards.

## Description
The Pet Medication Dose Calculator provides an advisory tool for calculating estimated medication dosages for pets. By providing the pet's weight in kilograms and selecting a supported medication, you can determine the therapeutic dosage range in milligrams. This MCP server includes tools such as `list_available_medications` to browse supported drugs, `get_dosage_range` to check mg/kg thresholds, and `calculate_medication_dose` for precise weight-based calculations. All calculations are based on hardcoded veterinary standards and must be verified by a licensed veterinarian.


## Available Tools (3)
- **get_dosage_range**: Get dosage range for a medication
- **list_available_medications**: List all available medications
- **calculate_medication_dose**: Calculate estimated dose for a pet


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Medication Dose Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What medications can I calculate doses for?"

**🤖 AI Agent:**
> The available medications are: Metamizole, Omeprazole, and Metronidazole.

---

**👤 You:**
> "What is the dosage range for Omeprazole?"

**🤖 AI Agent:**
> The recommended dosage range for Omeprazole is 0.5 to 1.0 mg/kg.

---

**👤 You:**
> "Calculate the dose for a 5kg dog using Metronidazole."

**🤖 AI Agent:**
> For a 5kg pet, the estimated dose of Metronidazole is between 12.5 mg and 25.0 mg. Please consult your veterinarian.


## ❓ FAQ

**Q: What medications are supported?**
You can use the `list_available_medications` tool to see a complete list of all drugs currently in our registry.

**Q: Is this calculation accurate for my pet?**
These calculations are strictly advisory and intended for educational purposes. Always confirm the dose with a licensed veterinarian before administration.

**Q: How do I calculate a specific dose?**
Use the `calculate_medication_dose` tool by providing the medication name and the pet's weight in kilograms.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pet-medication-dose-calculator](https://vinkius.com/mcp/pet-medication-dose-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Medication Dose Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-medication-dose-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Medication Dose Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-medication-dose-calculator": {
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
