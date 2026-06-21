# NFe.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nfeio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Orchestrate NFe.io services — manage service invoices (NFS-e), validate city codes, and monitor company data directly from any AI agent.

## Description
Connect your AI agents to **NFe.io**, the leading Brazilian platform for fiscal document automation. This MCP provides 10 tools to manage the full lifecycle of Service Invoices (NFS-e), validate Brazilian municipal codes (IBGE), and monitor corporate metadata for companies integrated into your billing environment.

### What you can do

- **Invoice Orchestration** — Issue, cancel, and retrieve Service Invoices (NFS-e) for multiple cities across Brazil
- **Company Management** — List and inspect registered companies and their current fiscal configurations
- **Service Definition** — Manage service codes and tax metadata to ensure accurate fiscal reporting
- **Fiscal Intelligence** — Retrieve detailed city capabilities and validate IBGE codes for seamless municipal integration
- **PDF Retrieval** — Generate and retrieve download links for official invoice PDF and XML documents programmatically

### How it works

1. Subscribe to this server
2. Log in to your [**NFe.io Dashboard**](https://nfe.io/)
3. Navigate to **API Settings** to obtain your **API Key**
4. Identify your **Company ID** for the specific issuing entity
5. Insert your credentials into the fields below to start managing your Brazilian fiscal workflows.

### Who is this for?

- **Brazilian SaaS Developers** — automate the issuance of recurring service invoices via AI workflows
- **Accountants & Finance Teams** — quickly retrieve monthly invoice summaries and XML files via natural language


## Available Tools (10)
- **cancel_service_invoice**: Cancel an issued Service Invoice (NFS-e)
- **create_company**: Register a new company (issuer) in NFe.io
- **get_company_details**: Get detailed info for a specific company issuer
- **get_merchandise_invoice**: Retrieve details for a specific Merchandise Invoice (NF-e)
- **get_service_invoice**: Retrieve details for a specific Service Invoice (NFS-e)
- **issue_merchandise_invoice**: Issue a Merchandise Invoice (NF-e)
- **issue_service_invoice**: Issue a Service Invoice (NFS-e)
- **list_companies**: List all companies (issuers) registered in your NFe.io account
- **list_webhooks**: List all configured webhooks in NFe.io
- **cancel_merchandise_invoice**: Cancel an issued Merchandise Invoice (NF-e)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NFe.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active companies in my NFe.io account."

**🤖 AI Agent:**
> I've retrieved your company list. You have 2 active entities: 1. Tech Services Ltda (ID: comp_1), 2. Consulting Group (ID: comp_2). Which one would you like to use for invoice issuance?

---

**👤 You:**
> "Check the status of service invoice ID 'inv_nfe_999888'."

**🤖 AI Agent:**
> Connecting to NFe.io gateway... Invoice 'inv_nfe_999888' is currently 'Issued' (Autorizada). I've found the official download links: [Download PDF](...) and [Download XML](...). Would you like me to send these to you?

---

**👤 You:**
> "Find the IBGE code for the city of 'São Paulo'."

**🤖 AI Agent:**
> Searching municipal codes... I found the IBGE code for São Paulo (SP): `3550308`. This code is active and compatible with the NFe.io service invoice engine.


## ❓ FAQ

**Q: Can my AI automatically issue an NFS-e for a specific customer?**
Yes! Use the `issue_service_invoice` tool with the Company ID and a JSON payload containing the customer data and service values. Your agent will trigger the issuance process with the relevant municipality.

**Q: How do I find the correct IBGE code for a Brazilian city?**
You can use the `list_cities` tool to search for municipalities by name or state. The agent will return the official IBGE codes required for fiscal document validation.

**Q: Can I retrieve the download link for an invoice PDF?**
Yes! Use the `get_service_invoice` tool with the unique Invoice ID. Your agent will return the metadata, including official links to download the PDF and XML versions of the document.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nfeio](https://vinkius.com/mcp/nfeio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NFe.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nfeio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NFe.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nfeio": {
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
