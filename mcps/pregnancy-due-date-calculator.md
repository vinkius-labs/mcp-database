# Pregnancy Due Date Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/pregnancy-due-date-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate estimated due dates, gestational age, and clinical milestones.

## Description
This MCP server provides deterministic pregnancy dating tools. Use `calculate_due_date` to find your estimated due date (EDD) using your last menstrual period (LMP), conception date, or ultrasound CRL measurements. You can also use `get_gestational_status` to track your current trimester and upcoming milestones, or `convert_crl_to_age` to translate ultrasound measurements into gestational weeks.


## Available Tools (3)
- **calculate_due_date**: Calculates the estimated due date and gestational progress based on LMP, conception, or ultrasound
- **convert_crl_to_age**: Converts a Crown-Rump Length (CRL) measurement into gestational age
- **get_gestational_status**: Provides a detailed breakdown of the current pregnancy stage and upcoming milestones


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pregnancy Due Date Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "When is my due date if my last menstrual period was on 2024-01-01 and my cycle is 28 days?"

**🤖 AI Agent:**
> Your estimated due date is 2024-10-08.

---

**👤 You:**
> "I had an ultrasound with a CRL of 15mm. How far along am I?"

**🤖 AI Agent:**
> Based on a CRL of 15mm, your gestational age is 0 weeks and 57 days (approximately 8 weeks and 1 day).

---

**👤 You:**
> "What is my current status if my pregnancy started on 2024-05-01?"

**🤖 AI Agent:**
> You are currently in your 2nd trimester, at 12 weeks and 3 days.


## ❓ FAQ

**Q: How do I calculate my due date using LMP?**
You can use the `calculate_due_date` tool with the 'lmp' input type and provide your last menstrual period date.

**Q: Can I use ultrasound measurements?**
Yes, use the `calculate_due_date` tool with the 'ultrasound' input type and provide the Crown-Rump Length (CRL) in millimeters.

**Q: What information is provided about my pregnancy progress?**
The tools provide your current gestational age in weeks and days, your current trimester, and upcoming clinical milestones.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/pregnancy-due-date-calculator](https://vinkius.com/ai-agent-connect/pregnancy-due-date-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pregnancy Due Date Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pregnancy-due-date-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pregnancy Due Date Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pregnancy-due-date-calculator": {
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
