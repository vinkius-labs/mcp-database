# Pediatric Dose Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pediatric-dose-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Calculate safe pediatric medication dosages based on weight and frequency.

## Description
This MCP server provides a precise calculation engine for determining safe pediatric medication dosages. By using the `get_drug_dosage_specs` tool, you can retrieve pharmacological constraints like minimum and maximum mg/kg thresholds. The `calculate_single_dose` tool allows for calculating the exact amount of medication needed for one administration based on a child's weight. For complex schedules, use `evaluate_dosage_regimem` to check total daily intake and identify potential overdose risks, ensuring the dosage stays within safe therapeutic windows.


## Available Tools (3)
- **calculate_single_dose**: Calculate a single dose based on weight
- **evaluate_dosage_regimen**: Evaluate a dosing schedule for safety
- **get_drug_dosage_specs**: Retrieve pharmacological constraints for a medication


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pediatric Dose Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the dosage limits for Paracetamol?"

**🤖 AI Agent:**
> For Paracetamol, the minimum dose is 10 mg/kg, the maximum single dose is 15 mg/kg, and the daily safety limit is 75 mg/kg.

---

**👤 You:**
> "Calculate a single dose of Ibuprofen for a child weighing 12kg."

**🤖 AI Agent:**
> The calculated dose for 12kg is 180 mg.

---

**👤 You:**
> "Is it safe to give Amoxicillin 3 times a day to a 5kg child, with each dose being 250mg?"

**🤖 AI Agent:**
> Danger: The total daily dose of 750mg exceeds the safety limit for a 5kg child.


## ❓ FAQ

**Q: How do I find the dosage limits for a specific drug?**
Use the `get_drug_dosage_specs` tool and provide the exact name of the medication as it appears in our registry.

**Q: Can this tool help prevent medication errors?**
Yes. By using `evaluate_dosage_regimen`, the system checks if the total daily dose exceeds safety thresholds and provides a 'Danger' warning if an overdose risk is detected.

**Q: What information do I need to calculate a single dose?**
You only need the name of the medication and the child's weight in kilograms to use the `calculate_single_dose` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pediatric-dose-calculator](https://vinkius.com/mcp/pediatric-dose-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pediatric Dose Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pediatric-dose-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pediatric Dose Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pediatric-dose-calculator": {
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
