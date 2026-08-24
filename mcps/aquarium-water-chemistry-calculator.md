# Aquarium Water Chemistry Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/aquarium-water-chemistry-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate precise chemical dosages for freshwater aquariums.

## Description
This MCP server provides precise tools for managing freshwater aquarium water chemistry. Use `calculate_dosing_plan` to determine the exact milliliters of chemical products needed to reach target GH, KH, pH, or Nitrate levels based on your tank volume. The server also includes `validate_parameter_ranges` to ensure your water readings are within safe biological limits and `get_product_efficacy` to look up the strength of specific additives. It automatically evaluates safety, providing warnings if proposed shifts in KH or pH exceed safe daily limits to prevent osmotic shock.


## Available Tools (3)
- **calculate_dosing_plan**: Calculates the exact volume of chemical products required to reach target parameters and evaluates the safety of the proposed shift
- **get_product_efficacy**: Retrieves the specific concentration/strength data for a single chemical product from the catalog
- **validate_parameter_ranges**: Checks if the provided current and target parameters are within biologically plausible or physically possible ranges


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aquarium Water Chemistry Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a 100L tank with GH 4, KH 3, pH 7.0, and Nitrate 20. I want to reach GH 6 and KH 5. How much should I dose?"

**🤖 AI Agent:**
> To reach your target parameters in a 100L tank, you should dose 20ml of GH+ and 15ml of KH+.

---

**👤 You:**
> "Check if a pH of 15 is valid for my aquarium."

**🤖 AI Agent:**
> No, a pH of 15 is not a valid parameter as pH must be between 0 and 14.

---

**👤 You:**
> "What is the efficacy of the product 'GH+'?"

**🤖 AI Agent:**
> GH+ raises GH by 3 dGH per 10ml per 50L.


## ❓ FAQ

**Q: How do I know if my dosing plan is safe?**
The `calculate_dosing_plan` tool automatically checks if the requested change in KH or pH exceeds safe daily limits and will provide a safety warning if the shift is too rapid.

**Q: Can I use this to check if my pH is too high?**
Yes, you can use `validate_parameter_ranges` to check if your current pH and other parameters are within biologically plausible ranges.

**Q: What products can I include in my calculation?**
You can include any product listed in the internal catalog. Use `get_product_efficacy` to find the exact name and strength of a product before including it in your dosing plan.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/aquarium-water-chemistry-calculator](https://vinkius.com/ai-agent-connect/aquarium-water-chemistry-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aquarium Water Chemistry Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aquarium-water-chemistry-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aquarium Water Chemistry Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aquarium-water-chemistry-calculator": {
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
