# PayFit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/payfit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Automate HR and payroll operations via PayFit — list collaborators, fetch payslips securely, overview company structure, and export accounting entries via AI.

## Description
Bring **PayFit Global Payroll** into your automated AI workflows natively. Providing a strict programmatic bridge to your company's HR and accounting infrastructure, this agent dynamically maps active employees, monitors valid compliance contracts, securely extracts monthly payslip distributions, and generates valid accounting entries directly via chat.

### What you can do

- **Company Overview** — Identify exact corporate metadata determining mapping addresses, strict payroll limits, and department structures implicitly
- **Collaborator Navigation** — Locate specific team boundaries, retrieving exactly which individual holds which contract running securely across active modules
- **Payslip Operations** — Identify discrete payslip runs fetching securely masked data tracking payroll compliance outputs
- **Ledger Generation** — Execute direct extractions generating valid mapping endpoints matching automated `accounting` metrics and financial records

### How it works

1. Subscribe to this server
2. Enter your PayFit Company ID and active API Key properly
3. Start validating dynamic accounting arrays directly with Claude, Cursor, or your preferred agent

### Who is this for?

- **Finance Teams** — seamlessly fetch bulk accounting records extracting arrays dynamically straight into ERP ingestion pipelines
- **People Operations** — audit active collaborator boundaries understanding precise module access and contract states instantly
- **Corporate Administrators** — build compliance workflows isolating departments strictly running explicit checks on mapped lists


## Available Tools (7)
- **get_company**: Get overview information about the PayFit company account
- **list_collaborators**: List all collaborators (employees) in the company
- **get_collaborator_details**: Get detailed information about a specific collaborator
- **list_contracts**: List all employment contracts in the company
- **list_payslips**: List all payslips for a specific collaborator
- **list_departments**: List all departments in the company
- **get_accounting_entries**: Get accounting entries for a specific payroll period (YYYYMM format)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PayFit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch the metadata configuration belonging to our main running PayFit company entity."

**🤖 AI Agent:**
> Connected successfully via `get_company`. The explicit bounds show entity 'Vinkius Global'. Registration country boundary set internally to 'FR'. Total active modules detected natively: 4. Would you like me to parse the connected departments next?

---

**👤 You:**
> "Scan our active architecture fetching a strict list of all collaborators and contracts."

**🤖 AI Agent:**
> Invoked explicitly bounding lists targeting `collaborators`. The array returned 40 limits natively. 1: Alice Engineering (ID xy1...). 2: John Security (ID zw2...). I also pulled their relative contract states logic. Ask me specifically for Alice's limits.

---

**👤 You:**
> "Retrieve global accounting transactions executed during March."

**🤖 AI Agent:**
> Pulled exact structures hitting `get_accounting_entries`. The payload reveals 12 distinct localized payroll ledger objects matching explicit debit and credit rules. Should I serialize these dynamically strictly into a table visual format for your review?


## ❓ FAQ

**Q: Can I automatically fetch raw PDF files of individual payslips?**
Currently the AI fetches structured JSON metadata representing the explicit payslip limits generated in the pay run, rather than arbitrary PDF media binaries. This ensures high-speed, secure token-based programmatic observation.

**Q: Do I need special scopes permitted via PayFit's platform security?**
Yes. Ensure the API token generated internally on PayFit's Admin panel is bound physically to 'Collaborators', 'Payslips', and 'Accounting' read boundaries. Without the proper scope, the endpoints strictly deny payloads.

**Q: How do accounting entries handle multiple logical company subsidiaries?**
The tool bounds its exact logic based directly on the explicit `Company ID` provided in the plugin settings. To query disparate subsidiaries, adjust the Company ID dynamically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/payfit](https://vinkius.com/mcp/payfit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PayFit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `payfit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PayFit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "payfit": {
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
