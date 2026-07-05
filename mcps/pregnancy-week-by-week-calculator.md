# Pregnancy Week-by-Week Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pregnancy-week-by-week-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Track pregnancy progress, fetal development milestones, and trimester symptoms.

## Description
The Pregnancy Week-by-Week Calculator connects AI agents to essential obstetric data. Using `calculate_pregnancy_status`, you can determine your current week, day, and upcoming milestones like viability and full term. The `get_weekly_development_data` tool provides fascinating weekly updates including fetal size comparisons to fruits or vegetables and key biological changes. Additionally, `get_trimester_information` helps users understand common physical and emotional symptoms throughout the First, Second, and Third trimesters.


## Available Tools (3)
- **calculate_pregnancy_status**: Calculates current pregnancy progress and upcoming milestones
- **get_trimester_information**: Provides common symptoms for a specific trimester
- **get_weekly_development_data**: Retrieves developmental milestones and size comparison for a specific week


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pregnancy Week-by-Week Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I had my last period on 2024-01-01. How far along am I and when is my due date?"

**🤖 AI Agent:**
> Based on your LMP of January 1st, 2024, you are currently in week 20 of your pregnancy (Second Trimester). Your estimated due date is October 7th, 2024.

---

**👤 You:**
> "What is happening to my baby at week 12?"

**🤖 AI Agent:**
> At week 12, your baby is roughly the size of a lime. Key milestones include the development of vital organs and the beginning of active movement, though you might not feel it just yet.

---

**👤 You:**
> "What symptoms should I expect in my first trimester?"

**🤖 AI Agent:**
> During the First Trimester, common symptoms include nausea (morning sickness), fatigue, breast tenderness, and frequent urination.


## ❓ FAQ

**Q: How do I calculate my current pregnancy week?**
You can use the `calculate_pregnancy_status` tool by providing either your last menstrual period (LMP) or your estimated due date.

**Q: Does it provide information about fetal size?**
Yes, the `get_weekly_development_data` tool provides a fun and helpful comparison of your baby's size to common fruits or vegetables for every week.

**Q: Can I see symptoms for my current trimester?**
Absolutely. By using `get_trimester_information`, you can retrieve a list of common physical and emotional symptoms associated with your specific stage of pregnancy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pregnancy-week-by-week-calculator](https://vinkius.com/mcp/pregnancy-week-by-week-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pregnancy Week-by-Week Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pregnancy-week-by-week-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pregnancy Week-by-Week Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pregnancy-week-by-week-calculator": {
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
