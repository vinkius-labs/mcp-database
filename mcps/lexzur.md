# Lexzur MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lexzur)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage legal operations with contract lifecycle tracking, matter management, and compliance workflows for corporate legal teams.

## Description
Connect your **Lexzur** (formerly App4Legal) account to any AI agent and take full control of your legal practice management and automated case workflows through natural conversation.

### What you can do

- **Matter & Litigation Orchestration** — List and manage your entire portfolio of high-fidelity Corporate Matters and Litigation Cases programmatically, retrieving detailed status and metadata
- **Contact Intelligence** — Access your complete directory of high-fidelity contacts and companies to coordinate your organizational relationship ecosystem in real-time
- **Case Lifecycle Monitoring** — Access real-time updates for legal cases and retrieve high-fidelity history for specific matters directly through your agent
- **Legal Discovery Management** — Query specific matters or contacts using custom search filters to maintain a perfectly coordinated audit trail of your legal practice
- **Operational Monitoring** — Verify account-level API connectivity and monitor practice volume directly through your agent for instant performance reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Token** and **Instance URL** from your Lexzur dashboard (Settings > API)
3. Start orchestrating your legal practice from Claude, Cursor, or any MCP client

No more manual logging into complex legal dashboards or missing case updates. Your AI acts as your dedicated legal coordinator and matter architect.

### Who is this for?

- **Lawyers & Attorneys** — instantly retrieve case summaries and matter statuses using natural language commands
- **Legal Operations** — monitor practice health and verify contact metadata without leaving your workspace
- **Paralegals** — automate the management of corporate records and contact directories through simple AI queries


## Available Tools (10)
- **create_matter**: Create a new legal matter
- **get_matter**: Get details for a specific matter
- **list_companies**: List companies/clients
- **list_contacts**: List contacts
- **list_documents**: List uploaded documents
- **list_invoices**: List legal invoices
- **list_litigation**: List litigation cases
- **list_matters**: List legal matters
- **list_tasks**: List legal tasks
- **list_time_logs**: List time entries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lexzur** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active corporate matters in my Lexzur account."

**🤖 AI Agent:**
> I've retrieved your corporate matters. You currently have 15 active portfolios, including 'M&A Deal A' and 'Global Audit'. Would you like the detailed high-fidelity metadata for any of them?

---

**👤 You:**
> "Show the status of litigation case 'Case_123'."

**🤖 AI Agent:**
> Accessing case architecture... Case_123 is currently in the 'Trial' stage. The high-fidelity history shows the last update was yesterday regarding 'Evidence Submission'. Need help checking upcoming deadlines for this case?

---

**👤 You:**
> "Retrieve the contact details for company 'Acme Legal'."

**🤖 AI Agent:**
> Contact orchestrated! I've successfully retrieved the high-fidelity metadata for Acme Legal (ID: comp_789). They have 3 linked lawyers and 5 active matters. Shall I list the detailed history for this company?


## ❓ FAQ

**Q: How do I find my Lexzur API Token?**
Log in to your account, navigate to **Settings** > **API**, and copy your unique access token from the credentials section.

**Q: Can I retrieve litigation cases via AI?**
Yes! The `list_litigation_cases` tool allows your agent to retrieve high-fidelity data for all ongoing court cases in your Lexzur portfolio.

**Q: How do I search for a specific contact?**
Use the `list_lexzur_contacts` tool and provide search parameters to retrieve high-fidelity metadata for specific individuals or companies.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lexzur](https://vinkius.com/mcp/lexzur)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lexzur** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lexzur` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lexzur** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lexzur": {
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
