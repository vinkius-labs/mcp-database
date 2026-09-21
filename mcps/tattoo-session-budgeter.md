# Tattoo Session Budgeter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tattoo-session-budgeter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate comprehensive tattoo project costs, payment milestones, and break-even points.

## Description
This MCP server provides financial planning tools for tattoo artists and clients. It calculates the full financial obligation for multi-session projects using `calculate_project_total`, provides a schedule of when payments are due via `get_payment_milestones`, and determines the minimum hourly rate needed to cover overhead with `analyze_break_even`. It also allows for a detailed breakdown of individual session costs versus the total project using `summarize_session_costs`.


## Available Tools (4)
- **analyze_break_even**: Calculate the minimum hourly rate required to cover non-session costs
- **calculate_project_total**: Determine the full financial obligation for a complete tattoo project
- **get_payment_milestones**: Provide a schedule of when payments are required
- **summarize_session_costs**: Break down the cost of a single session versus the total project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tattoo Session Budgeter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the total cost for a 3-session tattoo project with a $150 hourly rate, 3 hours per session, a $50 minimum charge, $100 design fee, $50 deposit, $20 travel, $15 aftercare, 8% tax, and a 20% tip."

**🤖 AI Agent:**
> The total project cost is $1,713.60, which includes $1,350.00 in session costs, $100.00 design fee, $20.00 travel, and $15.00 aftercare, plus $108.00 in tax and $225.60 in tip.

---

**👤 You:**
> "What are the payment milestones for a project with a $200 deposit and 2 sessions costing $400 each?"

**🤖 AI Agent:**
> The milestones are: $200.00 deposit at the start, and $400.00 at the beginning of each of the 2 sessions.

---

**👤 You:**
> "Break down the costs for a single session where the hourly rate is $120 and the session is 2 hours, with a $200 minimum charge."

**🤖 AI Agent:**
> The single session cost is $200.00, as the minimum charge applies because the hourly rate of $240.00 is higher than the minimum, wait, actually the single session cost is $240.00.


## ❓ FAQ

**Q: How do I calculate the total cost of a multi-session tattoo?**
You can use the `calculate_project_total` tool. It takes into account session count, hourly rates, design fees, travel, supplies, taxes, and tips to provide a complete project total.

**Q: Can I see when I need to pay for each session?**
Yes, the `get_payment_milestones` tool generates a schedule of payments, including the initial deposit and subsequent session payments.

**Q: How can an artist determine their minimum required rate?**
Artists can use `analyze_break_even` to calculate the minimum hourly rate required to cover non-session-specific costs like design fees, travel, and aftercare.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tattoo-session-budgeter](https://vinkius.com/en/ai-agent-connect/tattoo-session-budgeter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tattoo Session Budgeter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tattoo-session-budgeter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tattoo Session Budgeter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tattoo-session-budgeter": {
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
