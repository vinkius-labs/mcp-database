# Salary to Hourly Rate Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/salary-to-hourly-rate-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Convert annual salary into hourly pay based on work hours and weeks per year.

## Description
This MCP server provides precise tools to convert annual compensation into hourly wages. It accounts for specific working schedules, including weekly hours and the total number of working weeks in a year. Use `calculate_hourly_rate` to find your hourly wage, `validate_work_schedule` to ensure your hours are within standard bounds, or `compare_hourly_rates` to decide between two different job offers. You can also use `get_standard_work_profiles` to quickly apply common templates like Full-Time or Part-Time schedules.


## Available Tools (4)
- **calculate_hourly_rate**: Calculates the hourly pay rate from a given annual salary and work schedule
- **compare_hourly_rates**: Compares two different salary structures to determine which offers a higher hourly wage
- **get_standard_work_profiles**: Provides common working templates to serve as baselines for calculations
- **validate_work_schedule**: Checks if a provided working schedule is logically sound and within standard bounds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salary to Hourly Rate Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my hourly rate if I earn $50,000 a year working 40 hours a week for 52 weeks?"

**🤖 AI Agent:**
> $24.04 per hour.

---

**👤 You:**
> "Compare an annual salary of $60,000 at 40 hours/week (52 weeks) vs $55,000 at 35 hours/week (52 weeks)."

**🤖 AI Agent:**
> The $60,000 salary at 40 hours per week is higher, offering $28.85 per hour compared to $30.22 per hour for the $55,000 option. Wait, let me re-calculate: $60,000 / (40*52) = $28.85; $55,000 / (35*52) = $30.22. The $55,000 salary at 35 hours per week is actually higher per hour.

---

**👤 You:**
> "Is a schedule of 50 hours per week and 52 weeks per year valid?"

**🤖 AI Agent:**
> Yes, that schedule is within the standard bounds.


## ❓ FAQ

**Q: How do I calculate my hourly rate?**
You can use the `calculate_hourly_rate` tool by providing your annual salary, the number of hours you work per week, and how many weeks you work per year.

**Q: Can I compare two different job offers?**
Yes, the `compare_hourly_rates` tool allows you to input the salary and schedule for two different options to see which one provides a higher hourly wage.

**Q: What are the standard work profiles available?**
You can use `get_standard_work_profiles` to access presets like Full-Time (40 hours/week, 52 weeks/year) and Part-Time (20 hours/week, 52 weeks/year).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/salary-to-hourly-rate-converter](https://vinkius.com/en/ai-agent-connect/salary-to-hourly-rate-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Salary to Hourly Rate Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `salary-to-hourly-rate-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Salary to Hourly Rate Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "salary-to-hourly-rate-converter": {
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
