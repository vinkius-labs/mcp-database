# Perfume Dilution Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/perfume-dilution-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Calculate exact carrier volumes and dilution ratios for perfume making.

## Description
A deterministic tool for perfumers to calculate the exact quantities of carrier fluids and fragrance oils required to reach specific concentration standards. Use `calculate_single_dilution` for individual oils, `calculate_blend_dilution` for mixing multiple oils, or `get_standard_concentration` to find industry ranges for Parfum, EDP, EDT, and Cologne.


## Available Tools (3)
- **get_standard_concentration**: Provides the midpoint concentration values for the industry-standard perfume categories
- **calculate_blend_dilution**: Calculates dilution requirements when mixing multiple different fragrance oils into a single base
- **calculate_single_dilution**: Determines the amount of carrier needed to dilute a single fragrance oil to a target concentration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Perfume Dilution Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much alcohol do I need to dilute 10g of oil to 20% concentration?"

**🤖 AI Agent:**
> To dilute 10g of oil to a 20% concentration using alcohol, you need 40.87 ml of carrier.

---

**👤 You:**
> "What is the standard range for an Eau de Parfum (EDP)?"

**🤖 AI Agent:**
> The standard range for Eau de Parfum (EDP) is 15% to 20%, with a midpoint of 17.5%.

---

**👤 You:**
> "I have 5g of oil A and 5g of oil B. How much oil carrier is needed for a 15% blend?"

**🤖 AI Agent:**
> For a 10g total oil blend at 15% concentration using carrier oil, you need 56.52 ml of carrier.


## ❓ FAQ

**Q: How do I calculate the carrier needed for a single oil?**
Use the `calculate_single_dilution` tool by providing the oil weight in grams, your target concentration, and the carrier type (alcohol, oil, or water).

**Q: Can I mix multiple oils at once?**
Yes, use `calculate_blend_dilution` to provide an array of weights for all oils in your blend to find the total carrier volume required.

**Q: What are the standard perfume concentrations?**
You can use `get_standard_concentration` to retrieve the midpoint and range values for Parfum, EDP, EDT, and Cologne.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/perfume-dilution-calculator](https://vinkius.com/ai-agent-connect/perfume-dilution-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Perfume Dilution Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `perfume-dilution-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Perfume Dilution Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "perfume-dilution-calculator": {
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
