# Moon Phase Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moon-phase-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate exact lunar phases, illumination percentages, and monthly schedules using astronomical algorithms.

## Description
The Moon Phase Calculator provides high-precision astronomical data for any given date. By utilizing a synodic month algorithm based on a reference New Moon, it calculates the exact lunar phase name (such as Full Moon or Waxing Crescent) and the precise illumination percentage of the moon's visible disk. Users can retrieve specific phase details using `calculate_phase`, generate a complete calendar of lunar events for any month with `generate_monthly_schedule`, or compare the brightness between two different dates using `compare_brightness`. This tool is ideal for astronomers, photographers, and anyone interested in tracking lunar cycles without relying on external APIs.


## Available Tools (3)
- **compare_brightness**: Determine which of two provided dates features a more brightly illuminated Moon
- **generate_monthly_schedule**: Provide a full calendar of lunar events and phases for a specific month and year
- **calculate_phase**: Retrieve the exact name of the lunar phase and its current brightness


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moon Phase Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the moon phase on July 4th, 2024?"

**🤖 AI Agent:**
> On July 4th, 2024, the Moon will be in the First Quarter phase with approximately 50% illumination.

---

**👤 You:**
> "Show me the lunar schedule for October 2024."

**🤖 AI Agent:**
> The lunar schedule for October 2024 includes: Oct 2 (New Moon), Oct 17 (Full Moon), and Oct 24 (Last Quarter).

---

**👤 You:**
> "Which date is brighter, August 1st or August 15th, 2024?"

**🤖 AI Agent:**
> August 15th, 2024 will be brighter, as the Moon is in its Waning Gibbous phase with higher illumination compared to August 1st.


## ❓ FAQ

**Q: How accurate are the lunar phase calculations?**
The calculations use a high-precision synodic month algorithm based on a known New Moon epoch, providing accurate phase names and illumination percentages.

**Q: Can I see the full moon schedule for next month?**
Yes, you can use the `generate_monthly_schedule` tool by providing the specific month and year to get a day-by-day breakdown of lunar phases.

**Q: Does this tool require an internet connection or external API?**
No, the calculations are performed locally using pure astronomical algorithms, ensuring privacy and reliability without external dependencies.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moon-phase-calculator](https://vinkius.com/mcp/moon-phase-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moon Phase Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `moon-phase-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moon Phase Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moon-phase-calculator": {
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
