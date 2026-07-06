# TaxBandits MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/taxbandits)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

File US tax forms electronically including W-2, 1099, and ACA forms with IRS-authorized e-filing and instant status tracking.

## Description
Connect your **TaxBandits** account to any AI agent and simplify how you manage tax filings, business records, and IRS submissions through natural conversation.

### What you can do

- **Business Management** — List all registered business entities and create new profiles for tax reporting purposes.
- **Tax Filing Oversight** — List and query filed or draft tax forms (e.g., 1099, W-2, 94x) across multiple tax years.
- **Submission Tracking** — Check the real-time status of your form submissions to ensure successful IRS or state delivery.
- **Transmission Monitoring** — List and inspect form transmissions to keep a record of your filing history.
- **Metadata Retrieval** — Fetch detailed metadata for specific businesses to verify identifiers like EIN and business addresses.
- **Compliance Automation** — Manage your tax reporting lifecycle directly from Claude, Cursor, or any MCP client.

### How it works

1. Subscribe to this server
2. Enter your TaxBandits Client ID and Client Secret (found in your developer portal)
3. Start managing your tax compliance from your favorite AI assistant

### Who is this for?

- **Accountants & CPAs** — quickly retrieve filing statuses and verify business metadata via simple AI commands.
- **Business Owners** — monitor the status of recurring tax forms and ensure compliance directly from the workspace.
- **Tax Software Developers** — test form creation and verify transmission logs via the AI assistant.


## Available Tools (6)
- **list_transmissions**: List form transmissions
- **create_business**: Pass data as a JSON string.

Create a new business entity
- **get_business_details**: Get specific business details
- **get_submission_status**: Check status of a form submission
- **list_businesses**: List all registered businesses
- **list_tax_forms**: Pass filters as a JSON string.

List tax forms (e.g. 1099)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TaxBandits** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all businesses registered in my account."

**🤖 AI Agent:**
> I've retrieved your business directory. You have 3 registered entities: 'Acme Corp' (EIN: XX-XXXX123), 'Tech Solutions LLC', and 'Global Logistics'. Which one would you like to see tax forms for?

---

**👤 You:**
> "Show me the 1099 forms filed for 'Acme Corp' in tax year 2023."

**🤖 AI Agent:**
> I've fetched the tax forms. For 'Acme Corp' in 2023, there are 5 filed 1099-NEC forms. Shall I retrieve the submission status for the latest batch?

---

**👤 You:**
> "Check the status of submission ID 'SUB-88231'."

**🤖 AI Agent:**
> Fetching status... Submission SUB-88231 is currently 'Accepted' by the IRS. The processing is complete and the confirmation has been logged. Is there anything else you need to verify?


## ❓ FAQ

**Q: Can I check the status of an IRS form submission via AI?**
Yes! Use the `get_submission_status` tool and provide the Submission ID. Your agent will retrieve the real-time status directly from TaxBandits.

**Q: How do I list all my registered businesses?**
Run the `list_businesses` query. The agent will retrieve a complete list of all business entities currently configured in your TaxBandits account.

**Q: Is it possible to see draft forms waiting to be filed?**
Absolutely. Use the `list_tax_forms` query. You can pass a JSON filter with the `TaxYear` and `FormType` to identify both filed and draft records.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/taxbandits](https://vinkius.com/mcp/taxbandits)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TaxBandits** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `taxbandits` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TaxBandits** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "taxbandits": {
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
