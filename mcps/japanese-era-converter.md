# Japanese Era Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/japanese-era-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Convert Gregorian dates to Japanese imperial eras and calculate era metrics.

## Description
This MCP server provides precise tools for navigating the Japanese imperial calendar (Gengo). It allows AI agents to determine the specific era name and year for any Gregorian date, calculate temporal metrics like days elapsed since an era began, and identify the zodiac animal for a given year. Use `convert_gregorian_to_era` to find the era name, `get_era_metrics` for duration data, and `get_zodiac_animal` for the zodiac cycle.


## Available Tools (3)
- **convert_gregorian_to_era**: Determine the Japanese era name and era year for a given Gregorian date
- **get_era_metrics**: Calculate temporal depth and total duration within a Japanese era
- **get_zodiac_animal**: g., 2024) to find its zodiac animal.

Identify the zodiac animal for a specific Gregorian year


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Japanese Era Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was the Japanese era for May 1, 2024?"

**🤖 AI Agent:**
> May 1, 2024 is in the Reiwa era, specifically Reiwa 6.

---

**👤 You:**
> "What is the zodiac animal for the year 2024?"

**🤖 AI Agent:**
> The zodiac animal for 2024 is the Dragon.

---

**👤 You:**
> "How many days have passed in the current era as of 2024-01-01?"

**🤖 AI Agent:**
> As of 2024-01-01, 1766 days have elapsed since the start of the Reiwa era.


## ❓ FAQ

**Q: What happens if I provide a date before the Meiji era?**
The tool will return an error indicating that the date is 'Pre-Meiji', as the converter only covers eras from Meiji onwards.

**Q: Can I find the zodiac animal for a specific year?**
Yes, you can use the `get_zodiac_animal` tool by providing the Gregorian year.

**Q: How are era metrics calculated?**
By using `get_era_metrics`, you can retrieve the total days elapsed since the era started and the total duration of the era to date.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/japanese-era-converter](https://vinkius.com/ai-agent-connect/japanese-era-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Japanese Era Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `japanese-era-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Japanese Era Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "japanese-era-converter": {
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
