# DISCO MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/disco)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Equip your AI agent to manage legal matters, track documents, and monitor review teams via the DISCO API.

## Description
Integrate **DISCO**, the leading legal technology platform, directly into your AI workflow. Manage your legal matters, monitor document ingestion and metadata, track document tags for review, and oversee your authorized users using natural language.

### What you can do

- **Matter Oversight** — List and retrieve detailed settings and statuses for all your legal matters in DISCO.
- **Document Intelligence** — Access full technical metadata for documents, including custodians and file properties.
- **Tag Management** — List and review document tags and taxonomies used for legal review and organization.
- **Review Team Monitoring** — Track authorized users and identify teams assigned to specific legal cases.

### How it works

1. Connect the DISCO integration to your AI assistant.
2. Authorize using your DISCO API Key and Client ID (found in your organization settings).
3. Orchestrate your legal discovery and matter management through intuitive conversation.

### Who is this for?

- **Legal Operations** — Quickly check matter statuses and document counts on the go.
- **Litigation Support** — Monitor document ingestion and tag applications via chat.
- **Attorneys & Paralegals** — Research document metadata and matter details during case planning.


## Available Tools
- **get_disco_account_metadata**: Retrieve metadata and usage limits for your DISCO account
- **get_document_metadata**: Get the full technical metadata for a specific document
- **get_matter_details**: Get detailed settings and information for a specific legal matter
- **list_matter_documents**: List all documents associated with a specific legal matter
- **list_matter_access_users**: List only the users who have explicit access to a specific matter
- **list_legal_matters**: List all legal matters in your DISCO account
- **list_recently_ingested_documents**: Identify documents that have been recently uploaded to a matter
- **list_document_tags**: List all tags used to categorize documents in a specific matter
- **list_authorized_users**: List all users with access to your DISCO account
- **search_matter_documents**: Search for specific keywords or metadata across documents in a matter


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DISCO** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active legal matters."

**🤖 AI Agent:**
> I've found 5 active matters in your DISCO account, including 'Smith vs. Jones' and 'Project Aurora Review'. Would you like to see the document count for the largest matter?

---

**👤 You:**
> "Show me the metadata for document 'DOC-9988'."

**🤖 AI Agent:**
> Document 'DOC-9988' was ingested on June 12th. The custodian is 'John Doe'. It is currently tagged as 'Privileged' and 'Highly Confidential'. Should I pull the full audit trail for this document?

---

**👤 You:**
> "Search for documents in 'Project Aurora' containing 'contract termination'."

**🤖 AI Agent:**
> I've found 3 documents in 'Project Aurora' matching 'contract termination'. They include an email thread and two PDF attachments. Would you like to see the tags applied to these results?


## ❓ FAQ

**Q: How do I get DISCO API credentials?**
Log in to your DISCO account, navigate to the organization settings, and you can generate or retrieve your API Key and Client ID from the API management section.

**Q: Can the agent download legal documents?**
This integration currently focuses on retrieving technical metadata and auditing document tags and statuses. Accessing full document content for download is managed via the DISCO platform.

**Q: Is the integration secure for sensitive legal data?**
Yes, it uses official DISCO API protocols and only accesses the matters and documents exposed via your API key permissions, ensuring enterprise-grade security.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/disco](https://vinkius.com/mcp/disco)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DISCO** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `disco` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DISCO** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "disco": {
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
