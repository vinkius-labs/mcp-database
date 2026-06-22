# Personal Year Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/personal-year-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Discover your numerological Personal Year, Month, and Day cycles with detailed forecasts.

## Description
This MCP server provides a complete numerological engine to calculate your individual energetic cycles. By using the `calculate_personal_year`, `calculate_personal_month`, and `calculate_personal_day` tools, you can uncover the core themes and predicted trends for any period in your life based on your birth date. The engine uses digit reduction to reveal the vibration of each cycle, offering insights into your personal trajectory.


## Available Tools (3)
- **calculate_personal_day**: Calculate the Numerology Personal Day
- **calculate_personal_month**: Calculate the Numerology Personal Month
- **calculate_personal_year**: Calculate the Numerology Personal Year


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Personal Year Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my numerology personal year if I was born on 1990-05-15 and the current year is 2024?"

**🤖 AI Agent:**
> Your Personal Year number is 8. The theme for this year is Power and Abundance, with a forecast focusing on financial management and material success.

---

**👤 You:**
> "What energy should I expect in May if my Personal Year is 8?"

**🤖 AI Agent:**
> Your Personal Month number for May is 4. The theme is Stability and Foundation, suggesting a focus on organization and hard work.

---

**👤 You:**
> "What is the energy for the 10th of the month if my Personal Month is 4?"

**🤖 AI Agent:**
> Your Personal Day number is 5. The theme is Change and Freedom, indicating a day of unexpected opportunities and movement.


## ❓ FAQ

**Q: How do I calculate my Personal Year?**
You can use the `calculate_personal_year` tool by providing your birth date in YYYY-MM-DD format and the current calendar year.

**Q: What is a Personal Month?**
A Personal Month is a specific monthly energy derived from your Personal Year number and the target month. Use `calculate_personal_month` to find its theme.

**Q: Can I calculate my daily energy?**
Yes, the `calculate_personal_day` tool allows you to determine the granular energy and trends for a specific day of the month.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/personal-year-calculator](https://vinkius.com/mcp/personal-year-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Personal Year Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `personal-year-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Personal Year Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "personal-year-calculator": {
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
