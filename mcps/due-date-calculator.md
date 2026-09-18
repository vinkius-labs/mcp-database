# Due Date Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/due-date-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate pregnancy due dates, trimesters, and milestones using Naegele's rule.

## Description
This MCP server provides precise obstetric calculations based on the Last Menstrual Period (LMP) and cycle length. It uses Naegele's rule with cycle length adjustments to provide accurate estimates. Use `get_due_date_summary` for a quick overview, `get_trimester_boundaries` to find stage dates, `get_pregnancy_milestones` for developmental events, and `get_gestational_progress_detail` for a deep dive into weeks and percentage completion.


## Available Tools (4)
- **get_due_date_summary**: Provides a comprehensive overview of the pregnancy status including the due date and current progress
- **get_gestational_progress_detail**: Provides a detailed breakdown of the current gestational age including percentage of pregnancy completed
- **get_pregnancy_milestones**: Provides key physiological or developmental milestones expected during the pregnancy
- **get_trimester_boundaries**: Identifies the start and end dates for each of the three pregnancy trimesters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Due Date Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "When is my due date if my last period was on 2024-01-01 and my cycle is 28 days?"

**🤖 AI Agent:**
> Your estimated due date is 2024-10-08.

---

**👤 You:**
> "What trimester am I in if my LMP was 2024-03-15 and my cycle is 30 days?"

**🤖 AI Agent:**
> You are currently in your Second Trimester.

---

**👤 You:**
> "Show me my pregnancy milestones for an LMP of 2024-05-10 and a 28-day cycle."

**🤖 AI Agent:**
> Key milestones include heartbeat detection around week 6 and major organ development around week 10.


## ❓ FAQ

**Q: How is the due date calculated?**
The due date is calculated using Naegele's rule, adjusted for your specific cycle length to ensure accuracy.

**Q: Can I adjust for a non-standard cycle length?**
Yes, you can provide your average cycle length to refine the calculations.

**Q: What information can I get about my pregnancy progress?**
You can retrieve your current trimester, gestational age in weeks and days, and key developmental milestones.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/due-date-calculator](https://vinkius.com/en/ai-agent-connect/due-date-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Due Date Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `due-date-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Due Date Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "due-date-calculator": {
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
