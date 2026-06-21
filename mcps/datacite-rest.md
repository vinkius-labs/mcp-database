# DataCite REST MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/datacite-rest)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Manage and query DOIs (Digital Object Identifiers) via DataCite — retrieve metadata, list activities, and manage research records directly from your AI agent.

## Description
Connect to the **DataCite REST API** to interact with the global infrastructure for research data. This MCP server allows your AI agent to search, retrieve, and manage DOIs and their associated metadata.

### What you can do

- **DOI Management** — Create, update, and delete DOI records (Draft state) with full JSON:API support.
- **Metadata Retrieval** — Fetch detailed metadata for any DOI, including affiliations and publisher info.
- **Search & Discovery** — List DOIs with advanced filtering by client, provider, prefix, or resource type.
- **Provenance & Events** — Track metadata changes through activities and discover citations or usage via events.
- **Infrastructure Overview** — List repository accounts (clients), providers, and prefixes within the DataCite network.

### How it works

1. Subscribe to this server
2. Enter your DataCite credentials (Username and Password)
3. Start managing research identifiers from Claude, Cursor, or any MCP-compatible client

No more manual searching through web portals to find research citations or metadata. Your AI acts as a dedicated research data manager.

### Who is this for?

- **Researchers & Academics** — instantly retrieve metadata and citations for specific datasets or publications
- **Data Librarians** — manage DOI records and verify metadata provenance directly from their workflow
- **Developers** — integrate scholarly metadata and DOI registration into automated research pipelines


## Available Tools
- **create_doi**: Requires Member API authentication (Repository account). Payload must follow JSON:API format.

Create a new DOI record
- **delete_doi**: Only DOIs in Draft state can be deleted. Requires Member API authentication.

Delete a DOI (Draft state only)
- **get_doi**: Retrieve metadata for a specific DOI
- **get_heartbeat**: Check API status
- **list_activities**: Retrieve metadata provenance (history of changes)
- **list_clients**: List DataCite Repository accounts
- **list_dois**: Retrieve a list of DOIs
- **list_events**: Retrieve links between DOIs and other resources (citations, usage)
- **list_prefixes**: List DOI prefixes
- **list_providers**: List DataCite Members and Consortium Organizations
- **list_reports**: List usage reports
- **update_doi**: Requires Member API authentication. Only included attributes will be updated.

Update an existing DOI record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DataCite REST** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the metadata for DOI 10.14454/qdd3-ps68."

**🤖 AI Agent:**
> I've retrieved the metadata for DOI 10.14454/qdd3-ps68. It refers to 'DataCite Content Negotiation' published by DataCite. Would you like to see the full list of creators or the associated resource type?

---

**👤 You:**
> "Search for DOIs related to 'climate change' from the last year."

**🤖 AI Agent:**
> I found several DOIs matching 'climate change'. Notable records include datasets from various repositories. I can filter these by resource type or provider if you'd like to narrow it down.

---

**👤 You:**
> "List the events or citations associated with DOI 10.14454/qdd3-ps68."

**🤖 AI Agent:**
> Fetching events... I've found the links between this DOI and other resources, including citations and usage metrics recorded in the DataCite Event Data system.


## ❓ FAQ

**Q: Can I search for DOIs using specific metadata queries?**
Yes! Use the `list_dois` tool with the `query` parameter. You can use OpenSearch query string syntax to search through all metadata fields indexed by DataCite.

**Q: How do I see the history of changes for a DOI?**
You can use the `list_activities` tool to retrieve metadata provenance, which shows the history of changes and updates made to records in the DataCite system.

**Q: Can I delete any DOI record?**
No. According to DataCite rules, only DOIs in the 'Draft' state can be deleted using the `delete_doi` tool. Registered or Findable DOIs cannot be deleted to ensure the persistence of research citations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/datacite-rest](https://vinkius.com/mcp/datacite-rest)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DataCite REST** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `datacite-rest` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DataCite REST** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "datacite-rest": {
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
