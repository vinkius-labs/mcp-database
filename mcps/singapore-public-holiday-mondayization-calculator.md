# Singapore Public Holiday & Mondayization Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/singapore-public-holiday-mondayization-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate Singapore public holiday impacts and Mondayization eligibility.

## Description
This MCP server provides deterministic calculations for Singapore public holidays based on the Employment Act. It determines if a holiday triggers 'Mondayization' (a substitute holiday) if it falls on a non-working day like Sunday. Use `get_holiday_details` to check specific dates, `get_work_schedule_info` to validate employee schedules, or `calculate_annual_holiday_summary` for a yearly overview of paid holidays and substitute events.


## Available Tools (3)
- **calculate_annual_holiday_summary**: Provides a high-level count of all paid holidays in a year for a specific schedule
- **get_work_schedule_info**: Validates and describes the properties of an employee's work schedule
- **get_holiday_details**: Determines the specific day of the week and holiday impact for a single given date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Singapore Public Holiday & Mondayization Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "If a public holiday falls on Sunday, 2024-01-01, and my schedule is Mon-Fri, what happens?"

**🤖 AI Agent:**
> The holiday falls on a Sunday. Since you do not work on Sundays, you are eligible for Mondayization. The substitute holiday date is 2024-01-02.

---

**👤 You:**
> "What is my work schedule info for 'Tue-Sat'?"

**🤖 AI Agent:**
> Your working days are Tuesday, Wednesday, Thursday, Friday, and Saturday. You work 5 days per week and Sunday is not included in your schedule.

---

**👤 You:**
> "How many paid holidays will I have in 2024 if I work Mon-Fri?"

**🤖 AI Agent:**
> In 2024, with a Mon-Fri schedule, you will have 11 paid holidays, including any substitute holidays triggered by Mondayization.


## ❓ FAQ

**Q: What is Mondayization?**
Mondayization occurs when a public holiday falls on a day that is not a normal working day for an employee, such as a Sunday. In such cases, the tool identifies eligibility for a substitute holiday on the following Monday.

**Q: How do I check my total paid holidays for the year?**
You can use the `calculate_annual_holiday_summary` tool by providing the target year and your work schedule to get a full count of paid holidays and Mondayization events.

**Q: Which AI clients can use this tool?**
This tool is compatible with Cursor, VS Code, Claude Desktop, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/singapore-public-holiday-mondayization-calculator](https://vinkius.com/ai-agent-connect/singapore-public-holiday-mondayization-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Singapore Public Holiday & Mondayization Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `singapore-public-holiday-mondayization-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Singapore Public Holiday & Mondayization Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "singapore-public-holiday-mondayization-calculator": {
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
