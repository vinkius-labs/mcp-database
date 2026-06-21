# Middesk MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/middesk)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Business identity verification — verify entities, Secretary of State records, and tax registrations via Middesk.

## Description
Connect your **Middesk** account to automate Business Identity (KYB) and compliance workflows. This server provides comprehensive access to Middesk's verification engine.

### What you can do

- **Entity Verification** — Create and monitor business verification requests with real-time status
- **Document Retrieval** — Access official Secretary of State filings and corporate documents
- **Smart Prefill** — Automatically populate business details from a single identifier like EIN or website
- **Tax Registration** — Manage and track state tax registrations and payroll compliance
- **Identity Autocomplete** — Search for businesses with live SOS record suggestions

### How it works

1. Subscribe to this server
2. Enter your **Middesk API Key**
3. Start verifying businesses directly from Claude, Cursor, or any MCP client


## Available Tools
- **autocomplete_identity**: Autocomplete business identity
- **create_business**: Requires legal name.

Create a new business verification
- **get_business**: Get a specific business
- **get_document**: Get a specific document
- **get_tax_registration**: Get a specific tax registration
- **list_businesses**: List all businesses
- **list_documents**: List documents for a business
- **list_tax_registrations**: List tax registrations
- **prefill_business**: g., website).

Prefill business details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Middesk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Verify the business 'Acme Corp' located in Delaware."

**🤖 AI Agent:**
> Initiating verification for Acme Corp... Submission ID #99882. I will monitor the status for you.

---

**👤 You:**
> "Find SOS filings for business ID 'bus_123'."

**🤖 AI Agent:**
> Retrieving documents... Found 2 filings: Articles of Incorporation and Statement of Information.


## ❓ FAQ

**Q: Where do I find my Middesk API Key?**
Log in to your Middesk Dashboard, go to Settings > Developer > Credentials to find your secret keys.

**Q: Does this support the Sandbox environment?**
Yes, you can use your 'mk_test_...' keys to interact with the Middesk Sandbox.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/middesk](https://vinkius.com/mcp/middesk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Middesk** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `middesk` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Middesk** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "middesk": {
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
