# Menstrual Cycle Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/menstrual-cycle-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Track menstrual cycle phases and identify fertile windows using historical period data.

## Description
This MCP server provides precise biological timeline predictions. By using tools like `get_cycle_phases`, `get_fertile_window`, and `predict_next_period_event`, users can accurately track the Menstrual, Follicular, Ovulatory, and Luteal phases of their cycle. The calculator uses the start date of the last period and average cycle duration to identify fertile windows and predict upcoming milestones.


## Available Tools (3)
- **get_cycle_phases**: Retrieves a detailed timeline of all four biological phases for the upcoming cycle
- **get_fertile_window**: Identifies the specific date range during which conception is most likely
- **predict_next_period_event**: Provides a quick look at the next major milestones in the user's cycle


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Menstrual Cycle Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "When is my next fertile window if my last period started on 2024-05-01 and my cycle is 28 days?"

**🤖 AI Agent:**
> Your fertile window is predicted to be from 2024-05-11 to 2024-05-16.

---

**👤 You:**
> "What are the phases of my current cycle starting from 2024-06-10 with a 30-day duration?"

**🤖 AI Agent:**
> Your cycle includes the Menstrual, Follicular, Ovulatory, and Luteal phases starting from 2024-06-10.

---

**👤 You:**
> "Predict my next period event based on a last period start date of 2024-01-15 and a 28-day cycle."

**🤖 AI Agent:**
> Your next period is predicted for 2024-02-12, with ovulation estimated around 2024-01-28.


## ❓ FAQ

**Q: How do I use the cycle phase tool?**
Provide the date of your last period in YYYY-MM-DD format and your average cycle length using the `get_cycle_phases` tool.

**Q: How is the fertile window calculated?**
The `get_fertile_window` tool identifies the range surrounding your predicted ovulation date based on your cycle history.

**Q: Can I predict my next period date?**
Yes, use the `predict_next_period_event` tool to see your predicted next period and ovulation dates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/menstrual-cycle-calculator](https://vinkius.com/mcp/menstrual-cycle-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Menstrual Cycle Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `menstrual-cycle-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Menstrual Cycle Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "menstrual-cycle-calculator": {
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
