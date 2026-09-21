# Remote.com MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/remotecom)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Query your Remote.com HRIS from any AI workflow — employments, leave, timesheets, payslips, expenses, invoices, payroll runs and hiring reference data.

## Description
Connect your **Remote.com** account to any AI agent so it can answer people-ops questions straight from your global HRIS — using Remote's official API.

### What you can do

- **Roster** — list employees and contractors, filter by status and type, then pull full detail (salary, contract terms, role, contact data) for one employment
- **Time-off** — read leave-policy balances and time-off requests with status and leave type
- **Work & money** — timesheets, payslips, expense claims and contractor invoices
- **Payroll** — list monthly payroll runs and their status per company
- **Reference data** — the countries Remote can hire and pay in, plus their public holidays, to plan an Employer-of-Record hire

### How it works

1. Subscribe to this server
2. Generate a company API token in Remote → **Company Settings → Integrations & APIs**
3. Ask your agent: "Who is on leave next week?", "Show me September payroll status", "Which contractors have unpaid invoices?"

The token is read-only scoped to your company. Tokens are environment-bound — an `ra_live_` token works against production, an `ra_test_` token against the sandbox.

### Who is this for

- **People-ops & HRIS admins** — answer headcount and payroll questions from a chat or automation instead of exporting spreadsheets
- **Finance ops** — reconcile invoices, expenses and payslips against other systems
- **Founders & operators** — check hiring-country feasibility and holiday calendars while planning a cross-border hire


## Available Tools (14)
- **get_employment**: Find the employment id with list_employments first.

Get full details for one employment
- **get_employment_basic_information**: Shares the same employment id.

Get the v2 basic-information profile for one employment
- **list_company_departments**: List departments for a company
- **list_contractor_invoices**: Only contractor employments produce invoices.

List contractor invoices
- **list_countries**: Use it to plan where an Employer-of-Record hire is possible before creating an employment.

List the countries Remote can hire and pay in
- **list_expenses**: The Remote API takes no employment_id or status filter on this endpoint — match records to an employment client-side.

List expense claims
- **list_payroll_runs**: Filter by payroll_period (YYYY-MM). Status is draft/processing/paid.

List payroll runs
- **list_timeoff**: Dates are ISO (YYYY-MM-DD).

List time-off requests
- **list_timesheets**: The Remote API takes no employment_id filter on this endpoint — fetch by status and match records to an employment client-side.

List timesheet entries
- **get_leave_policy_summary**: Covers what the deprecated timeoff-balances endpoint used to return.

Summarize the leave policy balances for one employment
- **list_companies**: Use external_id to look up a single company by your own identifier.

List the companies in your Remote account
- **list_country_holidays**: Pass the country code from list_countries and a 4-digit year.

List the public holidays for a country
- **list_employments**: Pass a higher `page` to continue. Filter with status=active and employment_type to narrow the roster.

List employees and contractors at the company
- **list_payslips**: List payslips


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Remote.com** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many active employees do we have, and what countries are they in?"

**🤖 AI Agent:**
> You have 47 active employees across 9 countries — the largest cohorts are the US (14), Germany (8) and Brazil (6). I filtered the roster by status=active and grouped by country.

---

**👤 You:**
> "Which contractors have invoices issued but not yet paid?"

**🤖 AI Agent:**
> Three contractors have unpaid invoices totalling $18,400 — two are in approved status awaiting payout, one is still pending approval. I listed contractor invoices for this quarter and matched them back to the contractor roster.

---

**👤 You:**
> "Which public holidays fall in Portugal in 2026? I need them for our leave policy."

**🤖 AI Agent:**
> Passing PT and 2026 returns the national holidays, fixed and movable: New Year on 1 Jan, Good Friday on 3 Apr, Freedom Day on 25 Apr, Labour Day on 1 May, Portugal Day on 10 Jun, Corpus Christi on 4 Jun, Assumption on 15 Aug, Republic Day on 5 Oct, All Saints on 1 Nov, Immaculate Conception on 8 Dec and Christmas on 25 Dec. Pass a subdivision code as well if you also want the regional holidays for Madeira or the Azores.


## ❓ FAQ

**Q: Where do I get my Remote API token?**
Sign in to Remote, open **Company Settings → Integrations & APIs** and generate a company API token. Tokens are environment-bound: an `ra_live_` token only works against production, and an `ra_test_` token only against the sandbox.

**Q: Can this server create or change records in Remote?**
No. This server only reads Remote's list and show endpoints — employments, leave, timesheets, payslips, expenses, invoices, payroll runs and reference data. Nothing is written or deleted.

**Q: Why did the API reject a filter I passed, like employment_id on timesheets?**
Remote's endpoints do not all accept the same filters — for example timesheets takes only status, and expenses takes none. The instructions on each tool state exactly which filters that endpoint supports; if a filter is missing, fetch the wider list and match records by id.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/remotecom](https://vinkius.com/en/ai-agent-connect/remotecom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Remote.com** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `remotecom` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Remote.com** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "remotecom": {
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
