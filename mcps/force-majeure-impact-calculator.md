# Force Majeure Impact Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/force-majeure-impact-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [legal](../categories/legal.md)

Calculate the legal and operational impact of Force Majeure events on contract obligations.

## Description
This MCP server provides tools to assess how Force Majeure events affect contractual duties. Using `calculate_suspension_period`, you can determine when obligations are expected to resume based on event start dates and estimated durations. The `determine_notice_deadline` tool identifies the critical window for formal notification, accounting for differences between US Common Law and EU Civil Law jurisdictions. Finally, `evaluate_termination_trigger` helps identify if an event's duration has reached the threshold required to exercise termination rights for Service, Supply, or Construction contracts.


## Available Tools
- **calculate_suspension_period**: Determines the exact date when the suspension of contractual obligations is expected to end
- **determine_notice_deadline**: Identifies the final date by which the affected party must formally notify the counterparty
- **evaluate_termination_trigger**: Determines if the prolonged nature of the event has reached the threshold for termination


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Force Majeure Impact Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "An event started on 2024-01-01 and is expected to last 20 days. When will obligations resume?"

**🤖 AI Agent:**
> You can use `calculate_suspension_period` with eventStartDate: '2024-01-01' and estimatedDurationDays: 20 to find the end date.

---

**👤 You:**
> "A construction contract event started on 2024-05-10 and has lasted 45 days. Can I terminate?"

**🤖 AI Agent:**
> Using `evaluate_termination_trigger` with eventDurationDays: 45, contractType: 'CONSTRUCTION', and jurisdiction: 'US_COMMON_LAW' will show that the threshold (90 days) has not yet been reached.

---

**👤 You:**
> "What is the notice deadline for a US contract that started yesterday?"

**🤖 AI Agent:**
> The `determine_notice_deadline` tool will calculate the 7-day window required for US Common Law jurisdictions.


## ❓ FAQ

**Q: How can I find out when my contract obligations will resume?**
Use the `calculate_suspension_period` tool by providing the event start date and the estimated duration in days.

**Q: What is the deadline for notifying a counterparty of an event?**
The `determine_notice_deadline` tool calculates this based on whether the contract follows US Common Law (7-day window) or EU Civil Law (14-day window).

**Q: Can I check if I have the right to terminate a contract?**
Yes. Use `evaluate_termination_trigger` with the current event duration and your contract type (Service, Supply, or Construction) to see if the threshold has been met.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/force-majeure-impact-calculator](https://vinkius.com/mcp/force-majeure-impact-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Force Majeure Impact Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `force-majeure-impact-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Force Majeure Impact Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "force-majeure-impact-calculator": {
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
