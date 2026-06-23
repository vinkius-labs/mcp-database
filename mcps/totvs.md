# TOTVS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/totvs)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Orchestrate TOTVS ERP services — manage employees, handle financials, and monitor BPM workflows directly from any AI agent.

## Description
Connect your AI agents to **TOTVS**, the largest technology company in Brazil and Latin America. This MCP provides 10 tools to manage organizational data across Protheus, RM, and Fluig ecosystems, enabling seamless orchestration of HR, Financial, and Business Process Management (BPM) workflows.

### What you can do

- **HR Orchestration** — List employees and retrieve detailed profiles across the organization
- **Financial Control** — Monitor accounts payable/receivable and list real-time receipts and payments
- **BPM Workflows** — Track and advance process requests in Fluig and manage the Electronic Content Management (ECM) system
- **Multi-System Access** — Unified interaction with Protheus, RM, and Fluig through a single AI interface

### How it works

1. Subscribe to this server
2. Log in to your [**TOTVS Portal**](https://www.totvs.com/)
3. Navigate to **Web Services / API Settings** in your ERP (Protheus/RM) or Fluig instance
4. Obtain your **Username**, **Password**, and **Base URL**
5. Identify your **Tenant ID** or **Company ID** if required
6. Connect your account to Vurb to start managing your enterprise data.

### Who is this for?

- **HR Business Partners** — quickly retrieve employee data and monitor leave trends via natural language
- **Finance Teams** — automate the monitoring of accounts and payment statuses smoothly
- **Process Analysts** — track and advance business workflows across the organizational ecosystem


## Available Tools (11)
- **get_available_services**: List available RM DataServers
- **get_employee_details**: Get detailed information for a specific employee
- **get_process_request**: Get details for a specific Fluig process request
- **get_rm_data**: Query a specific record from an RM DataServer
- **list_companies**: List all companies and branches in the Protheus environment
- **list_documents**: List documents in the Fluig ECM
- **list_employees**: List employees from the HR module
- **list_payments**: List accounts payable (Finance)
- **list_processes**: List all BPM processes in Fluig
- **list_receipts**: List accounts receivable (Finance)
- **move_process_request**: Advance a Fluig process request to the next state


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TOTVS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active employees in my TOTVS RM environment."

**🤖 AI Agent:**
> Retrieving employee list from RM... I've found 150 active records. Key roles include Software Engineers, Account Managers, and HR Specialists. Would you like the detailed profile for a specific person?

---

**👤 You:**
> "Show the accounts payable summary for this month from Protheus."

**🤖 AI Agent:**
> Connecting to Protheus financials... For April 2024, you have 45 pending payments totaling R$ 125,400.00. 12 are overdue. Would you like me to list the overdue invoices?

---

**👤 You:**
> "List all pending workflow requests in Fluig."

**🤖 AI Agent:**
> Fetching Fluig task list... I found 8 pending requests: 1. Purchase Requisition #101, 2. Vacation Request #202, 3. Travel Expense #303... Which one would you like to advance?


## ❓ FAQ

**Q: Which TOTVS systems are compatible with this MCP?**
This MCP is designed to work with standard REST APIs from Protheus, RM, and Fluig. Ensure your specific instance has the relevant API modules enabled.

**Q: How do I find my TOTVS Base URL?**
The Base URL is the address of your ERP or Fluig web service (e.g., `https://erp.mycompany.com:8080/rest`). You can find this in your system's technical documentation or environment settings.

**Q: Can I automatically advance a Fluig process request?**
Yes! Use the `advance_process` tool with the specific Process Instance ID. Your agent will trigger the workflow transition based on the logic defined in Fluig.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/totvs](https://vinkius.com/mcp/totvs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TOTVS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `totvs` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TOTVS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "totvs": {
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
