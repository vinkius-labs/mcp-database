# Documint MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/documint)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to automate document generation, manage templates, and track output files via the Documint API.

## Description
Integrate **Documint**, the versatile document generation and automation platform, directly into your AI workflow. Manage your dynamic document templates, generate professional PDF files from JSON data, and track your generation history using natural language.

### What you can do

- **Template Oversight** — List and retrieve detailed configuration and variable schemas for all your document templates.
- **Document Generation** — Trigger the Documint engine to create new files instantly using provided data variables.
- **Generation Tracking** — Monitor the status of your document generations and access secure download URLs.
- **Variable Intelligence** — Identify exactly which data keys are required to populate specific templates accurately.

### How it works

1. Connect the Documint integration to your AI assistant.
2. Authorize using your Documint API Key (found in your account settings).
3. Orchestrate your document automation and reporting through intuitive conversation.

### Who is this for?

- **Operations Managers** — Quickly generate invoices or proposals from CRM data on the go.
- **Accountants** — Monitor document generation status and access output files for billing via chat.
- **Developers** — Audit template variables and test document generation logic instantly.


## Available Tools
- **create_new_generation**: Generate a new document using a specific template and data object
- **get_documint_account_metadata**: Retrieve metadata and usage limits for your Documint account
- **get_generation_details**: Get the current status and download URL for a specific generated document
- **get_template_variable_audit**: Identify exactly which variables are required to populate a template
- **get_template_configuration**: Get detailed information and field schema for a specific template
- **list_documint_generations**: List all documents that have been generated in Documint
- **list_failed_doc_generations**: Identify document generations that failed due to errors (mock logic)
- **list_latest_doc_generations**: Identify the most recently generated documents
- **list_documint_templates**: List all available document templates in your Documint account
- **search_documint_templates**: Search for a document template using a name keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Documint** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available Documint templates."

**🤖 AI Agent:**
> I've found 4 templates in your account, including 'Q3 Sales Proposal', 'Client Onboarding Pack', and 'Event Ticket'. Would you like to see the required variables for the Sales Proposal?

---

**👤 You:**
> "Generate a new 'Event Ticket' with data: {'guest_name': 'Jane Smith', 'seat': 'A12'}."

**🤖 AI Agent:**
> I've triggered the generation for 'Event Ticket'. The document is being processed. I'll provide the download URL as soon as it's ready. The document ID is 'DOCUMINT-7788'.

---

**👤 You:**
> "Show me the status of the last 5 generations."

**🤖 AI Agent:**
> Your last 5 generations were all 'Completed' successfully. Documents include: 'Proposal_TechCorp.pdf', 'Ticket_JaneSmith.pdf', and 'Invoice_99.pdf'. Would you like the download links for any of these?


## ❓ FAQ

**Q: How do I get a Documint API Key?**
Log in to your Documint account, navigate to the API section in your account settings, and you can generate or retrieve your unique API Key from there.

**Q: Can the agent show me the variables for a template?**
Yes, you can use the get_template_variable_audit tool to retrieve exactly which data keys are needed to populate a specific template.

**Q: What format are the documents generated in?**
Documint specializes in generating high-quality PDF files from your dynamic HTML or designed templates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/documint](https://vinkius.com/mcp/documint)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Documint** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `documint` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Documint** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "documint": {
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
