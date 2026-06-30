# Sun Sign Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sun-sign-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Calculate precise zodiac signs with year-specific cusp transitions and astrological properties.

## Description
The Sun Sign Calculator provides highly accurate astrological data by calculating zodiac sign cusps based on the specific birth year. Unlike static date ranges, this tool accounts for orbital variations to identify the exact start and end dates of a sign's period. Use `calculate_cusp` to find your sign's boundaries and `get_sign_details` to retrieve elemental, modal, and polarity attributes like Fire, Earth, Cardinal, or Masculine.


## Available Tools (2)
- **get_sign_details**: Get elemental and modal properties of a zodiac sign
- **calculate_cusp**: Calculate the zodiac sign cusp for a given date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sun Sign Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my zodiac sign if I was born on March 20, 1995?"

**🤖 AI Agent:**
> On March 20, 1995, your zodiac sign was Pisces. The cusp period for that year began on February 19 and ended on March 20.

---

**👤 You:**
> "Tell me the properties of the Aries sign."

**🤖 AI Agent:**
> Aries is characterized by the Fire element, the Cardinal modality, and a Masculine polarity.

---

**👤 You:**
> "What are the boundaries for the sign of Leo in 2024?"

**🤖 AI Agent:**
> In 2024, the period for Leo begins on July 22 and ends on August 22.


## ❓ FAQ

**Q: Why do I need to provide my birth year?**
Zodiac sign transitions (cusps) do not occur on the same calendar day every year due to Earth's orbital variations. Providing the year ensures the `calculate_cusp` tool identifies the precise boundaries for your specific birth period.

**Q: What information can I get about a zodiac sign?**
By using `get_sign_details`, you can retrieve the fundamental astrological attributes of any sign, including its element (e.g., Fire, Water), modality (e.g., Cardinal, Fixed), and polarity (e.g., Masculine, Feminine).

**Q: Can this tool calculate my full astrological profile?**
Yes, by combining the `calculate_cusp` and `get_sign_details` tools, you can determine your sign's boundaries and its corresponding elemental and modal characteristics for a complete identity summary.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sun-sign-calculator](https://vinkius.com/mcp/sun-sign-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sun Sign Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sun-sign-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sun Sign Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sun-sign-calculator": {
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
