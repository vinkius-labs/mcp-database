# Pregnancy Due Date Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pregnancy-due-date-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate gestational age, due dates, and prenatal schedules using LMP, IVF, or ultrasound data.

## Description
The Pregnancy Due Date Engine provides precise clinical calculations for pregnancy progress. By connecting your AI agent to this MCP server, you can determine the Estimated Due Date (EDD), current gestational weeks and days, and trimester status using various biological markers including Last Menstrual Period (LMP), conception date, IVF transfer dates (with Day 3 or Day 5 embryo adjustments), and ultrasound Crown-Rumb Length (CRL) measurements. Additionally, use `get_fetal_growth_metrics` to estimate fetal weight percentiles and `get_pregnancy_milestones` to identify critical clinical landmarks like viability and full term. The engine also automates the ACOG prenatal visit schedule via `get_prenatal_visit_schedule`, ensuring all upcoming medical appointments are tracked accurately.


## Available Tools (4)
- **get_fetal_growth_metrics**: Estimate fetal weight percentile
- **calculate_gestational_status**: Calculate pregnancy progress and due date
- **get_pregnancy_milestones**: Get key pregnancy milestones
- **get_prenatal_visit_schedule**: Generate upcoming prenatal visit schedule


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pregnancy Due Date Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Based on my LMP of 2024-01-01, what is my estimated due date and current progress?"

**🤖 AI Agent:**
> Your Estimated Due Date (EDD) is 2024-10-07. You are currently in your second trimester, at 25 weeks and 3 days of gestation.

---

**👤 You:**
> "I had an IVF transfer on 2024-03-15 with a Day 5 embryo. When is my due date?"

**🤖 AI Agent:**
> Your Estimated Due Date (EDD) is 2024-12-01.

---

**👤 You:**
> "What are my upcoming prenatal visit weeks based on being 12 weeks and 2 days pregnant?"

**🤖 AI Agent:**
> Your next scheduled visits are at week 14, week 16, and week 18.


## ❓ FAQ

**Q: How can I calculate my due date using IVF transfer information?**
You can use the `calculate_gestational_status` tool by providing your `ivfTransferDate` and specifying whether it was a Day 3 or Day 5 embryo using the `embryoAgeDays` parameter.

**Q: Can this engine help with tracking prenatal appointments?**
Yes, the `get_prenatal_visit_schedule` tool calculates upcoming medical visits based on the ACOG standard schedule using your current gestational age.

**Q: Does the engine support ultrasound measurements?**
Yes, you can provide a Crown-Rump Length (CRL) measurement in millimeters via the `ultrasoundCrlMm` parameter in the `calculate_gestational_status` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pregnancy-due-date-engine](https://vinkius.com/mcp/pregnancy-due-date-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pregnancy Due Date Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pregnancy-due-date-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pregnancy Due Date Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pregnancy-due-date-engine": {
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
