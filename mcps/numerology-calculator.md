# Numerology Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/numerology-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Get a complete Pythagorean numerology profile including Life Path, Destiny, and Soul Urge numbers.

## Description
This MCP server provides a deterministic Pythagorean numerology engine. It calculates core life profile numbers such as the Life Path, Destiny/Expression, Soul Urge, Personality, and Birthday numbers. The engine respects Master Numbers (11, 22, 33) and identifies Karmic Debt numbers (13, 14, 16, 19) during the reduction process. Use `calculate_numerology_profile` for a full analysis or `get_name_vibration` to focus on name-based vibrations.

### Available Tools

`calculate_numerology_tool`, `get_name_vibration_tool`, `validate_date_integrity_tool`


## Available Tools (3)
- **validate_date_integrity_tool**: Verifies if a provided birth date is chronologically possible and follows standard formatting
- **calculate_numerology_tool**: Provides a complete numerological analysis for an individual based on their identity and birth details
- **get_name_vibration_tool**: Analyzes only the vibrational components of a name (Soul Urge and Personality) without requiring a birth date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Numerology Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you calculate my numerology profile? My name is John Doe and I was born on 1990-05-15."

**🤖 AI Agent:**
> Your Life Path Number is 3, your Destiny Number is 1, your Soul Urge is 5, and your Personality Number is 6.

---

**👤 You:**
> "What is the vibration of the name Jane Smith?"

**🤖 AI Agent:**
> For Jane Smith, the Soul Urge is 7, the Personality is 4, and the Destiny vibration is 2.

---

**👤 You:**
> "Is 1995-02-30 a valid birth date?"

**🤖 AI Agent:**
> No, that is not a valid date.


## ❓ FAQ

**Q: What is a Life Path number?**
The Life Path number is derived from your birth date and represents the core journey and traits you carry through life. Tools available: `calculate_numerology_tool`, `get_name_vibration_tool`, `validate_date_integrity_tool`.

**Q: What are Master Numbers?**
Master Numbers are 11, 22, and 33. In this system, they are high-vibration numbers that are not reduced to single digits.

**Q: How do I get a full profile?**
You can use the `calculate_numerology_profile` tool by providing your first name, last name, and birth date in YYYY-MM-DD format.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/numerology-calculator](https://vinkius.com/ai-agent-connect/numerology-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Numerology Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `numerology-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Numerology Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "numerology-calculator": {
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
