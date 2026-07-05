# Supplement Dosage Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/supplement-dosage-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate precise supplement dosages based on body weight, age, sex, and ingredient chemistry.

## Description
The Supplement Dosage Calculator is an expert system designed to bridge the gap between elemental nutrient requirements and actual compound mass. It provides highly accurate dosing instructions for key supplements like Vitamin D, Magnesium, Iron, and Creatine by accounting for physiological metrics such as body weight, age, and hemoglobin levels. Using tools like `calculate_vitamin_d_dose`, `calculate_magnesium_mass`, `calculate_iron_dosage`, and `calculate_creatine_regimen`, users can determine the exact amount of a supplement compound needed to reach their target elemental dosage. The system also includes `lookup_supplement_safety_parameters` to retrieve official RDA and UL benchmarks, ensuring supplementation remains within safe physiological limits.


## Available Tools (5)
- **calculate_creatine_regimen**: Provides daily creatine dosing for both loading and maintenance phases
- **calculate_iron_dosage**: Determines the required dose of iron salts to address hemoglobin deficiency or maintain levels
- **calculate_magnesium_mass**: Calculates the total mass of a magnesium compound needed to achieve a specific elemental magnesium goal
- **lookup_supplement_safety_parameters**: Retrieves official safety and nutritional benchmarks for any supplement in the database
- **calculate_vitamin_d_dose**: Adjusts for deficiency.

Determines the daily Vitamin D requirement in both mcg and IU based on user physiology


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Supplement Dosage Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much magnesium glycinate should I take to get 200mg of elemental magnesium?"

**🤖 AI Agent:**
> To achieve a target of 200mg of elemental magnesium using the glycinate form, you need to consume approximately 1245.45mg of magnesium glycinate.

---

**👤 You:**
> "What is my Vitamin D dose if I weigh 80kg and am 30 years old?"

**🤖 AI Agent:**
> For a body weight of 80kg at age 30, the recommended dosage is 25mcg (1000 IU) per day.

---

**👤 You:**
> "I am starting a creatine loading phase. I weigh 75kg. How much do I need?"

**🤖 AI Agent:**
> For your 75kg body weight, the recommended loading phase dose is 15 grams of creatine per day.


## ❓ FAQ

**Q: How does the calculator handle different forms of magnesium?**
The `calculate_magnesium_mass` tool uses specific elemental yield percentages for various forms like glycinate, citrate, and oxide to calculate the total compound mass required.

**Q: Can I use this for Vitamin D conversions?**
Yes, `calculate_vitamin_d_dose` provides both micrograms (mcg) and International Units (IU) based on your body weight and age.

**Q: Does the tool provide safety information?**
Yes, you can use `lookup_supplement_safety_parameters` to find the Recommended Dietary Allowance (RDA) and Upper Limit (UL) for various supplements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/supplement-dosage-calculator](https://vinkius.com/mcp/supplement-dosage-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Supplement Dosage Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `supplement-dosage-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Supplement Dosage Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "supplement-dosage-calculator": {
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
