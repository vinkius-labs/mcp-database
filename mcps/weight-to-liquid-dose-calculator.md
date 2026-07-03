# Weight to Liquid Dose Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/weight-to-liquid-dose-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [healthcare](../categories/healthcare.md)

Calculate exact liquid medication volumes based on patient weight and concentration.

## Description
This MCP server provides precise clinical calculations for converting patient body mass into measurable liquid medication doses. By using tools like `calculate_mass_requirement`, `convert_mg_to_ml`, and `calculate_full_liquid_dose`, healthcare professionals can accurately determine the total milligrams required and the corresponding volume in milliliters to administer, based on specific drug concentrations. It eliminates manual calculation errors in weight-based dosing scenarios.


## Available Tools (3)
- **calculate_full_liquid_dose**: Calculate the final liquid volume to administer
- **calculate_mass_requirement**: Calculate the total milligrams of medication required based on patient weight
- **convert_mg_to_ml**: Convert a target mass of medication into the required liquid volume


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Weight to Liquid Dose Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "A child weighs 15kg. The prescribed dose is 10mg/kg. The concentration is 5mg/mL. How much liquid should I give?"

**🤖 AI Agent:**
> For a 15kg patient with a 10mg/kg dose and 5mg/mL concentration, the total mass required is 150mg, which equals a volume of 30mL.

---

**👤 You:**
> "How many milligrams of medication are needed for a 25kg patient at a dosage of 15mg/kg?"

**🤖 AI Agent:**
> The total mass requirement for a 25kg patient at 15mg/kg is 375mg.

---

**👤 You:**
> "If I have 100mg of medication and the concentration is 25mg/mL, what volume do I draw up?"

**🤖 AI Agent:**
> You should draw up 4mL of the liquid.


## ❓ FAQ

**Q: How does the tool handle different concentrations?**
You can use `convert_mg_to_ml` by providing the specific concentration (mg/mL) of your medication to find the exact volume needed.

**Q: Can I calculate both mass and volume at once?**
Yes, the `calculate_full_liquid_dose` tool performs both steps: it calculates the total required mass and then converts that mass into the final liquid volume.

**Q: What happens if I enter an invalid weight?**
The tool validates all inputs. If you provide a zero, negative, or non-numeric value for weight or dosage, the calculation will return an error to prevent unsafe dosing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/weight-to-liquid-dose-calculator](https://vinkius.com/mcp/weight-to-liquid-dose-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Weight to Liquid Dose Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `weight-to-liquid-dose-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Weight to Liquid Dose Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "weight-to-liquid-dose-calculator": {
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
