# Chuanyun MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chuanyun)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Enterprise workflow automation and digital engine — manage business objects, forms, and approval history via AI.

## Description
Empower your AI agent to orchestrate your enterprise digital infrastructure with **Chuanyun** (H3Yun), the leading low-code engine for rapid business digitalization. By connecting Chuanyun to your agent, you transform complex business object management and workflow auditing into a natural conversation. Your agent can instantly list your forms, retrieve field schemas, manage business records (create, update, delete), and even browse historical workflow approval steps without you ever needing to navigate the technical Chuanyun portal. Whether you are managing complex supply chain objects, customized ERP modules, or internal administrative tasks, your agent acts as a real-time digital engine, keeping your data accurate and your business logic optimized.

### What you can do

- **Form Orchestration** — List all accessible application schemas and retrieve detailed field definitions.
- **Business Object Control** — Manage business records (objects) with full support for batch listing, creation, and granular updates.
- **Workflow Auditing** — Check the defined workflows and historical approval history for any business object instance.
- **Schema Insights** — Retrieve internal schema codes and structures to understand your enterprise data architecture.
- **Team Coordination** — Access organization user lists to manage assignments and participation effectively.

### How it works

1. Subscribe to this server
2. Enter your Chuanyun Engine Code and Engine Secret
3. Start managing your digital infrastructure through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Business Analysts** — automate data collection and monitor business process execution through natural language.
- **Operations Managers** — oversee complex business objects and approval histories through a unified AI interface.
- **IT Administrators** — monitor application schemas and automated workflows without manual technical overhead.
- **Enterprise Power Users** — integrate your existing Chuanyun business logic into your AI-driven daily routines.


## Available Tools
- **create_biz_object**: Create a new business object
- **delete_biz_object**: Delete a business object
- **get_biz_object_details**: Get object detailed data
- **get_form_schema**: Get form field schema
- **get_workflow_history**: Get workflow instance history
- **list_biz_objects**: List business objects (records)
- **list_forms**: List all forms in the application
- **list_users**: List application users
- **list_workflows**: List form workflows
- **update_biz_object**: Update an existing business object


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chuanyun** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all business object forms available in my Chuanyun app."

**🤖 AI Agent:**
> I've retrieved the available forms for your Chuanyun application. You have 6 schemas, including 'Sales Orders', 'Material Procurement', and 'Customer Assets'. Which one would you like to view records for?

---

**👤 You:**
> "Show me the last 3 records from the 'Material Procurement' form (Code: D00123)."

**🤖 AI Agent:**
> I've listed the last 3 records from 'Material Procurement'. They include Procurement Order #P-8821, #P-8822, and #P-8823. Would you like to see the detailed field data for any of these orders?

---

**👤 You:**
> "Retrieve the approval history for sales order 'OBJ-9920'."

**🤖 AI Agent:**
> I've retrieved the approval history for 'OBJ-9920'. The order was approved by the Sales Manager at 9 AM and is currently pending with the Warehouse Director for final verification. Would you like a detailed step-by-step breakdown?


## ❓ FAQ

**Q: How do I find my Chuanyun Engine Code and Secret?**
Log in to the H3Yun Portal, go to [Settings] → [Integration] → [API], and you will find your Engine Code and Engine Secret (API Secret) there.

**Q: What is a 'Schema Code' in Chuanyun?**
A Schema Code is the unique identifier for a specific form or business object structure. You can find these codes in the application design section or by using the `list_forms` tool.

**Q: Can I see who approved a specific business object?**
Yes. Use the `get_workflow_history` tool with the business object ID. It will return the detailed history of the workflow, including all approval steps and the users involved.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chuanyun](https://vinkius.com/mcp/chuanyun)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chuanyun** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `chuanyun` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chuanyun** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chuanyun": {
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
