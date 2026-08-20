# Japanese Era & Zodiac Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/japanese-era-zodiac-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Convert Gregorian dates to Japanese eras and determine zodiac animals.

## Description
This MCP server provides precise tools for navigating the Japanese calendar system. You can use `convert_date_to_era` to transform any YYYY-MM-DD date into its specific Japanese era name and year, or `convert_era_to_date` to find the Gregorian equivalent of an era designation. It also includes `get_era_details` to retrieve historical timelines and durations for specific eras. Additionally, the service calculates the 12-year zodiac animal for any given year.


## Available Tools (3)
- **convert_date_to_era**: Converts a standard Gregorian date into its corresponding Japanese era name and era year
- **convert_era_to_date**: Converts a Japanese era designation into a standard Gregorian date
- **get_era_details**: Answers specific questions about the duration and timeline of an era


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Japanese Era & Zodiac Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was the Japanese era for 2023-05-20?"

**🤖 AI Agent:**
> The date 2023-05-20 falls in the Reiwa era, year 5. The zodiac animal for 2023 is the Rabbit.

---

**👤 You:**
> "Convert Reiwa 1, year 1 to a Gregorian date."

**🤖 AI Agent:**
> Reiwa year 1 corresponds to the Gregorian date 2019-05-01.

---

**👤 You:**
> "How long was the Heisei era?"

**🤖 AI Agent:**
> The Heisei era lasted for 30 years, starting from January 8, 1989.


## ❓ FAQ

**Q: What happens if I provide a date before the Meiji era?**
The `convert_date_to_era` tool will return 'Pre-Meiji' for any date occurring before September 8, 1868.

**Q: Can I convert a Reiwa year back to a Gregorian date?**
Yes, you can use the `convert_era_to_date` tool by providing 'Reiwa' as the era name and the specific year.

**Q: How is the zodiac animal determined?**
The zodiac animal is calculated based on the 12-year cycle (Rat, Ox, Tiger, etc.) corresponding to the Gregorian year.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/japanese-era-zodiac-converter](https://vinkius.com/ai-agent-connect/japanese-era-zodiac-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Japanese Era & Zodiac Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `japanese-era-zodiac-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Japanese Era & Zodiac Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "japanese-era-zodiac-converter": {
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
