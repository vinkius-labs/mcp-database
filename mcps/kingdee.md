# Kingdee / 金蝶 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kingdee)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Comprehensive enterprise ERP platform — manage materials, customers, and business flows via AI.

## Description
Empower your AI agent to orchestrate your entire enterprise operations with **Kingdee** (金蝶), the premier ERP platform in China. By connecting Kingdee to your agent, you transform complex business management, supply chain tracking, and financial auditing into a natural conversation. Your agent can instantly list master data forms, create or update records, monitor approval statuses, and execute complex business queries without you ever needing to navigate the comprehensive Kingdee Cloud Cosmic interface. Whether you are managing high-volume purchase orders or auditing customer records, your agent acts as a real-time operations assistant, keeping your ERP data accurate and your business flows moving.

### What you can do

- **Master Data Orchestration** — Manage materials, customers, and suppliers with full support for saving and viewing records.
- **Business Flow Control** — Submit, audit, and revoke approvals for any business form in your ERP system.
- **Advanced Querying** — Execute powerful business queries to retrieve specific datasets and perform trend analysis.
- **Status Conversion** — Trigger downstream business processes and status conversions directly through the agent.
- **Organization Insights** — Retrieve high-level information about your enterprise organizational units and data centers.

### How it works

1. Subscribe to this server
2. Enter your Kingdee API Host, Account ID (acctid), and App Credentials
3. Start managing your enterprise operations through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — monitor supply chain progress and audit master data through natural language queries.
- **Finance Teams** — coordinate approvals and track financial documents directly from your AI-powered workspace.
- **IT Administrators** — oversee organizational units and manage ERP integrations via a unified AI interface.
- **Kingdee Power Users** — integrate your existing ERP workflows into your AI-driven daily routines.


## Available Tools (10)
- **get_org_info**: Get organization metadata
- **list_forms**: List common ERP forms
- **query_data**: Execute business query
- **save_form**: Save/Create an ERP form
- **status_convert**: Convert form status
- **submit_form**: Submit ERP form
- **un_audit_form**: Un-audit/Revoke approval
- **view_form**: View ERP form details
- **audit_form**: Audit/Approve ERP form
- **delete_form**: Delete ERP form record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kingdee / 金蝶** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active purchase orders in Kingdee."

**🤖 AI Agent:**
> I've retrieved your active purchase orders. You have 12 open orders, including transactions for 'Steel Pipes' and 'Industrial Lubricants'. Would you like to check the approval status for any of them?

---

**👤 You:**
> "Get the details for material 'MAT-8821'."

**🤖 AI Agent:**
> I've retrieved the details for material MAT-8821. It is currently in stock with 500 units available in the 'Main Warehouse'. The status is 'Audited'. Would you like to see the linked supplier information?

---

**👤 You:**
> "Audit the sales orders 'SAL-9920' and 'SAL-9921'."

**🤖 AI Agent:**
> Done! I've successfully audited the specified sales orders. They are now marked as 'Approved' in your Kingdee ERP system and are ready for fulfillment.


## ❓ FAQ

**Q: How do I find my Kingdee Account ID (acctid)?**
Your Account ID (acctid) is the unique identifier for your Kingdee data center. You can find it on the login screen of your Kingdee Cloud instance or in the system management settings.

**Q: Can I perform business queries through this server?**
Yes. Use the `query_data` tool with the target form ID and field keys. You can also provide a filter string to retrieve specific subsets of your ERP data.

**Q: How do I audit/approve a record?**
Use the `audit_form` tool with the form ID and the comma-separated list of record IDs (Numbers) you wish to approve. Ensure the records have been successfully submitted first.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kingdee](https://vinkius.com/mcp/kingdee)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kingdee / 金蝶** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kingdee` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kingdee / 金蝶** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kingdee": {
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
