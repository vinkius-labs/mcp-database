# Flea & Tick Treatment Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flea-tick-treatment-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Calculate precise flea and tick medication dosages and administration schedules based on pet mass and product formulation.

## Description
This MCP server provides clinical utility for determining safe and effective pest control regimens. Using `calculate_dosage_window`, you can identify the required dosage range (mg/kg) and application frequency for different product types like spot-on, oral, or collars. The `get_weight_tier_metadata` tool maps pet mass to standardized commercial weight tiers, while `validate_treatment_safety` ensures that a specific dose of active ingredient falls within the therapeutic window for a given pet's weight.


## Available Tools (3)
- **calculate_dosage_window**: Determines the required dosage range and frequency
- **get_weight_tier_metadata**: ).

Identifies the weight tier for a given mass
- **validate_treatment_safety**: Checks if a specific dose is safe


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flea & Tick Treatment Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the dosage range and frequency for a 12kg dog using an oral treatment?"

**🤖 AI Agent:**
> For a 12kg dog using an oral formulation, the required dosage is between 5.0 mg/kg and 10.0 mg/kg, with an application interval of 30 days.

---

**👤 You:**
> "Is it safe to apply 50mg of active ingredient to a 3kg cat using spot-on treatment?"

**🤖 AI Agent:**
> No, applying 50mg to a 3kg cat results in approximately 16.67 mg/kg, which exceeds the maximum safe threshold for the Small weight tier.

---

**👤 You:**
> "What weight tier does a 25kg pet fall into?"

**🤖 AI Agent:**
> A 25kg pet is classified in the Large weight tier.


## ❓ FAQ

**Q: How do I calculate the correct dosage for my pet?**
Use the `calculate_dosage_window` tool by providing your pet's weight in kilograms and the product type (spot_on, oral, or collar). It will return the minimum and maximum safe dosage in mg/kg and the required application interval.

**Q: Can I verify if a specific dose is safe?**
Yes, use the `validate_treatment_safety` tool. Provide the pet's weight, the product type, and the total milligrams of active ingredient being administered to check if it falls within the safe therapeutic window.

**Q: How are weight tiers determined?**
The `get_weight_tier_metadata` tool identifies the standardized commercial tier (Small, Medium, Large, or Extra-Large) based on the pet's mass in kilograms.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flea-tick-treatment-calculator](https://vinkius.com/mcp/flea-tick-treatment-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flea & Tick Treatment Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flea-tick-treatment-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flea & Tick Treatment Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flea-tick-treatment-calculator": {
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
