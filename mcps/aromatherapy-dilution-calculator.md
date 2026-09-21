# Aromatherapy Dilution Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/aromatherapy-dilution-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate safe essential oil dilutions for massage therapy based on client profiles.

## Description
This MCP server provides professional tools for aromatherapy practitioners to ensure safe topical application of essential oils. It calculates precise dilution ratios, provides detailed safety profiles for individual oils, and validates application methods against specific client demographics like infants, pregnant individuals, or the elderly. Use `calculate_dilution_ratio` to determine exact drop counts for a specific volume of carrier oil, or `get_oil_safety_profile` to check for contraindications and skin sensitization risks.


## Available Tools (4)
- **calculate_dilution_ratio**: Determines the required number of essential oil drops and the resulting concentration for a specific volume of carrier oil
- **check_application_compatibility**: Validates if a specific application method is appropriate for the chosen client type
- **get_carrier_oil_options**: Lists available carrier oils and their characteristics to assist in selection
- **get_oil_safety_profile**: Provides specific safety data and warnings for a single essential oil


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aromatherapy Dilution Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many drops of Lavender oil should I add to 50ml of jojoba oil for a full-body massage on an adult?"

**🤖 AI Agent:**
> For 50ml of carrier oil for an adult full-body massage, you should add 10 drops of Lavender oil to achieve a safe 2% dilution.

---

**👤 You:**
> "Is it safe to use Peppermint oil on an infant?"

**🤖 AI Agent:**
> No, Peppermint oil is generally not recommended for infants due to high sensitization risks and strict safety thresholds for this demographic.

---

**👤 You:**
> "What are the contraindications for Tea Tree oil?"

**🤖 AI Agent:**
> Tea Tree oil should be avoided on broken skin and used with caution by individuals with known skin sensitivities.


## ❓ FAQ

**Q: How do I know if a dilution is safe for a child?**
You can use the `calculate_dilution_ratio` tool and specify 'child' as the client type. The tool automatically adjusts the maximum allowable percentage based on professional safety standards for children.

**Q: Can I check for specific oil contraindications?**
Yes, use the `get_oil_safety_profile` tool. It returns a list of contraindications and the maximum safe percentage for that specific essential oil.

**Q: Does this tool support different carrier oils?**
Yes, you can use `get_carrier_oil_options` to view available carrier oils and their absorption rates to help you choose the best base for your dilution.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/aromatherapy-dilution-calculator](https://vinkius.com/en/ai-agent-connect/aromatherapy-dilution-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aromatherapy Dilution Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aromatherapy-dilution-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aromatherapy Dilution Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aromatherapy-dilution-calculator": {
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
