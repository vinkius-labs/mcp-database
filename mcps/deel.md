# Deel MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deel)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage global contracts, team members, invoices, payments, time-off, and expenses — global HR for AI agents.

## Description
Integrate **Deel**, the all-in-one global people platform, directly into your AI workflow. Manage your international team, track contracts and compliance, monitor invoices and payments, and handle time-off requests using natural language.

### What you can do

- **Contract Management** — List and view contracts with terms, compensation, and compliance status across 150+ countries.
- **Global Team Directory** — Browse and retrieve profiles for all your employees and contractors in one unified view.
- **Payroll & Invoice Tracking** — Monitor invoices, view payment history, and track processing status for your global workforce.
- **Leave & Expense Oversight** — Monitor time-off requests and review submitted expenses with approval statuses.

### How it works

1. Connect the Deel integration to your AI assistant.
2. Authorize using your Deel API Token (found in your Developer settings).
3. Orchestrate your global HR operations through intuitive conversation.

### Who is this for?

- **HR Managers** — Quickly check contract statuses and team details on the go.
- **Finance Teams** — Monitor global payroll invoices and payment processing via chat.
- **Operations Leaders** — Track time-off and expenses across international entities effortlessly.


## Available Tools
- **list_contracts**: Returns contract metadata including legal type (e.g., fixed, PAYG, milestone), current status, and high-level compensation structures.

List all contracts
- **list_expenses**: Returns expense report metadata including receipt attachments, currency amounts, and the current review status (approved/rejected/pending).

List submitted expenses
- **get_contract**: Resolves detailed terms, compliance requirements, specific compensation rates, and effective dates.

Get contract details
- **list_people**: Returns a list of team members including their professional roles, geographical locations, and the nature of their Deel integration (employee vs. contractor).

List all people (employees and contractors)
- **get_person**: Resolves personal metadata, active and historical contract links, and cumulative payment history within the Deel platform.

Get person details
- **list_invoices**: Returns invoice metadata including billing amounts, issue dates, and current payment status (e.g., paid, pending, overdue).

List all invoices
- **list_payments**: Returns data on disbursement amounts, recipient identifiers, and the technical status of each transfer.

List all payments
- **list_time_off**: Returns a collection of time-off requests including requested dates, leave categories, and the current approval status for each entry.

List time-off requests
- **list_tasks**: Returns task descriptions, due dates, and completion status for milestone-based engagements.

List tasks for a contract
- **list_milestones**: Returns identifiers, payment amounts, and projected achievement dates for defined project stages.

List contract milestones


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active contractors in my team."

**🤖 AI Agent:**
> I've found 24 active contractors, including 'Maria Santos' (Brazil) and 'Kenji Tanaka' (Japan). Would you like to see the monthly compensation for any of them?

---

**👤 You:**
> "What invoices are currently pending payment?"

**🤖 AI Agent:**
> There are 5 pending invoices totaling $18,400. The largest is for 'Kenji Tanaka' ($8,000) due on April 10th. Should I pull the full payment report?

---

**👤 You:**
> "Show me any time-off requests pending approval."

**🤖 AI Agent:**
> I found 3 pending time-off requests: 'Alex Kim' (3 days in May), 'Sarah Lee' (1 week in June), and 'David Chen' (today). Would you like to see the reasons provided for these requests?


## ❓ FAQ

**Q: How do I get a Deel API Token?**
Log in to your Deel account, navigate to **Organization Settings** → **Developer Center** → **API Tokens**, and click **Create Token**.

**Q: Can I see all active contracts?**
Yes! You can use the list_contracts tool to see all contracts with their type, status, and compensation details across your entire organization.

**Q: How do I track payments to contractors?**
Use the list_payments tool to see full payment history, or list_invoices to track specific billing statuses and amounts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deel](https://vinkius.com/mcp/deel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Deel** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `deel` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deel** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deel": {
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
