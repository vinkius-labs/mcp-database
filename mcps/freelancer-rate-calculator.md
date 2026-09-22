# Freelancer Rate Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/freelancer-rate-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate sustainable hourly rates based on target income and billable capacity.

## Description
This MCP server provides essential financial planning tools for freelancers to bridge the gap between their desired income and their actual billable capacity. Use `get_required_rate` to determine the exact hourly rate needed to meet your annual goals, or `get_capacity_summary` to understand how your weekly work hours translate into annual billable time. You can also use `simulate_rate_impact` to model how changes in your capacity affect your rates, and `validate_sustainability` to check if your current rate is sufficient to cover your target income and business overhead.


## Available Tools (4)
- **get_capacity_summary**: Provides an overview of how a freelancer's time is distributed between billable and non-billable work
- **get_required_rate**: Calculates the hourly rate needed to reach a specific income target
- **simulate_rate_impact**: Allows a freelancer to see how changing their billable capacity or income target affects their required hourly rate
- **validate_sustainability**: Checks if a currently existing hourly rate is sufficient to meet a target income given a specific capacity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Freelancer Rate Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to earn $100,000 a year and I can work 1,200 billable hours. What should my hourly rate be?"

**🤖 AI Agent:**
> To earn $100,000 with 1,200 billable hours, your required hourly rate is $83.33.

---

**👤 You:**
> "I work 40 hours a week, 48 weeks a year, and 60% of my time is billable. How many billable hours do I have per year?"

**🤖 AI Agent:**
> You have 1,152 billable hours per year.

---

**👤 You:**
> "If I increase my billable hours from 1,000 to 1,200 for a $100,000 target, how much will my rate change?"

**🤖 AI Agent:**
> Your rate will decrease from $100.00 to $83.33, which is a 16.67% reduction.


## ❓ FAQ

**Q: How do I calculate my required hourly rate?**
You can use the `get_required_rate` tool by providing your target annual income, your total annual billable hours, and an optional operating margin for business expenses.

**Q: What is the difference between total hours and billable hours?**
Total hours include all time spent working, while billable hours are only the hours spent on client-facing, revenue-generating tasks. Use `get_capacity_summary` to see this breakdown.

**Q: Can I check if my current rate is enough to meet my goals?**
Yes, the `validate_sustainability` tool allows you to input your current rate and target income to see if you will meet your financial goals.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/freelancer-rate-calculator](https://vinkius.com/en/ai-agent-connect/freelancer-rate-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Freelancer Rate Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `freelancer-rate-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Freelancer Rate Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "freelancer-rate-calculator": {
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
