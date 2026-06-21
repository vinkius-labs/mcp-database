# Finch MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/finch)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Connect Finch to automate HRIS and Payroll integration — list employees, retrieve employment data, and manage pay statements directly from your AI agent.

## Description
Finch is the unified API for HRIS and payroll. This MCP server allows your AI agent to interact with various HR and payroll providers through a single integration flawlessly.

### Key Features
- **Directory Orchestration** — List all employees in the connected organization and fetch detailed profiles natively.
- **Employment Intelligence** — Retrieve granular employment data including job titles, departments, and compensation flawlessly.
- **Payroll Transparency** — Access pay groups and individual pay statements to monitor payroll data synchronously.
- **Connection Introspection** — Check the status, provider, and authorized permissions for any connection flawlessly native.
- **Automated Job Tracking** — Monitor data sync jobs to ensure your HRIS data is always up to date flawlessly through the agent.
- **Provider Discovery** — List all supported HRIS and payroll providers to verify integration compatibility flawlessly.

### How it works
1. Subscribe to this server
2. Enter your Finch Access Token (obtained via Finch Connect)
3. Start managing your HRIS and payroll data from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **HR Operations** — automate employee data retrieval and verification without manual portal exports
- **Finance Teams** — monitor payroll statements and compensation data directly from your chat workflow
- **Product Teams** — integrate unified HR data into your internal tools and workflows through simple natural language queries


## Available Tools (11)
- **get_automated_job**: Get details for a specific automated job
- **get_company**: Get organization data (legal name, EIN, primary address)
- **get_employment**: Get employment data for an individual (title, salary, department, etc.)
- **get_individual**: Get personal data for an individual (name, email, SSN, etc.)
- **get_me**: Get details for the authorized application/user connection
- **introspect**: Check the status and permissions of the current connection
- **list_automated_jobs**: List automated data sync jobs
- **list_directory**: Read the employee directory for the connected organization
- **list_pay_groups**: List pay groups for the organization
- **list_pay_statements**: List pay statements for a specific payment ID
- **list_supported_providers**: List all HRIS/Payroll providers supported by Finch


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Finch** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all employees in the directory."

**🤖 AI Agent:**
> I've retrieved the employee directory. You have 45 individuals registered, including 'Alice Johnson' (Marketing) and 'Bob Smith' (Engineering). Would you like to see the employment details for any of them?

---

**👤 You:**
> "Check the status of my connection to Gusto."

**🤖 AI Agent:**
> Introspecting connection... Your connection to Gusto is active and authorized. You have permissions for 'directory', 'employment', and 'payment'. Shall I fetch the latest organization metadata?

---

**👤 You:**
> "List pay statements for payment ID pmt_123."

**🤖 AI Agent:**
> Retrieving pay statements... For payment pmt_123, I found statements for 12 employees. The total gross pay was $54,000. Would you like to see the individual breakdown for any specific employee?


## ❓ FAQ

**Q: How do I obtain a Finch Access Token?**
Access tokens are generated when a user successfully completes the Finch Connect authorization flow for their specific HRIS or payroll provider.

**Q: Which HRIS providers does Finch support?**
Finch supports over 200 providers including Gusto, ADP, Workday, BambooHR, and Rippling. You can use the `list_supported_providers` tool to see the full list flawlessy.

**Q: Can I see individual pay statements?**
Yes! The `list_pay_statements` tool allows you to retrieve payment details for individuals if the connected organization has granted the necessary payroll permissions flawlessy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/finch](https://vinkius.com/mcp/finch)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Finch** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `finch` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Finch** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "finch": {
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
