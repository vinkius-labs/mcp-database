# Pregnancy Week Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pregnancy-week-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Track your pregnancy progress, from gestational age to weekly fetal milestones.

## Description
This MCP server provides essential tools for tracking pregnancy. Use `calculate_gestation` to find out how many weeks pregnant you are based on your last menstrual period or conception date. You can also use `get_due_date` to estimate your baby's arrival, `get_pregnancy_stage` to identify your current trimester, and `get_weekly_milestone` to learn about fetal development each week.


## Available Tools (4)
- **calculate_current_gestation**: Calculate current gestational age
- **get_estimated_due_date**: Get the estimated due date
- **get_pregnancy_stage**: Get the current pregnancy stage
- **get_weekly_milestone**: Get the weekly milestone


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pregnancy Week Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many weeks pregnant am I if my last period was January 1st, 2024?"

**🤖 AI Agent:**
> As of today, you are approximately 15 weeks and 3 days pregnant.

---

**👤 You:**
> "When is my baby due if my LMP was May 10th, 2024?"

**🤖 AI Agent:**
> Your estimated due date is February 13th, 2025.

---

**👤 You:**
> "What is happening with my baby at week 12?"

**🤖 AI Agent:**
> At week 12, your baby is about the size of a lime and important organs are continuing to develop.


## ❓ FAQ

**Q: How can I find out my current gestational age?**
Use the `calculate_gestation` tool by providing your last menstrual period or conception date.

**Q: Can I see what is happening with my baby this week?**
Yes, the `get_weekly_milestone` tool provides developmental updates and size comparisons for any specific week.

**Q: How do I know which trimester I am in?**
The `get_pregnancy_stage` tool calculates your current stage based on your pregnancy progress.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pregnancy-week-calculator](https://vinkius.com/mcp/pregnancy-week-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pregnancy Week Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pregnancy-week-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pregnancy Week Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pregnancy-week-calculator": {
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
