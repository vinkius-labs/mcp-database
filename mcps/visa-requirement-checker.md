# Visa Requirement Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/visa-requirement-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Check visa requirements, travel advisories, and passport validity rules globally.

## Description
The Visa Requirement Checker provides a comprehensive database for travelers. Use `check_visa_requirements` to find entry modes like e-Visa or Visa-free status. Check safety with `get_travel_advisory`. Verify health mandates using `check_entry_health_rules`, and ensure your passport meets the `get_passport_validity_rule` for your destination. It also includes `get_passport_power_info` to see your global mobility rank.


## Available Tools (5)
- **get_passport_power_info**: Gets passport power information
- **get_passport_validity_rule**: Gets the passport validity rule for a country
- **check_entry_health_rules**: Checks entry health rules
- **check_visa_requirements**: Checks visa requirements for a traveler
- **get_travel_advisory**: Gets the travel advisory for a country


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Visa Requirement Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Do I need a visa to travel from the USA to Japan?"

**🤖 AI Agent:**
> You can enter Japan with a US passport under Visa-Free status for up to 90 days.

---

**👤 You:**
> "What is the current travel advisory for France?"

**🤖 AI Agent:**
> The current advisory level for France is Low, meaning it is safe for typical travel with standard precautions.

---

**👤 You:**
> "How much validity does my passport need for Brazil?"

**🤖 AI Agent:**
> Brazil requires your passport to have at least 6 months of remaining validity.


## ❓ FAQ

**Q: How can I check if I need a visa for Japan?**
Use the `check_visa_requirements` tool by providing your passport country code and Japan's country code.

**Q: Does this tool cover vaccination requirements?**
Yes, the `check_entry_health_rules` tool provides information on mandatory vaccinations like Yellow Fever.

**Q: Can I check my passport power?**
Yes, use `get_passport_power_info` to see your global mobility rank and accessible destinations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/visa-requirement-checker](https://vinkius.com/mcp/visa-requirement-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Visa Requirement Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `visa-requirement-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Visa Requirement Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "visa-requirement-checker": {
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
