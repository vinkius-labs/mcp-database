# ORCID MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/orcid)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access and manage ORCID researcher records — search the registry, fetch biographical data, and manage works or affiliations directly.

## Description
Connect to the **ORCID** (Open Researcher and Contributor ID) registry to identify and connect researchers with their professional activities across disciplines and borders.

### What you can do

- **Record Retrieval** — Fetch full summary views or specific biographical sections of any researcher using their 16-digit ORCID iD.
- **Activity Tracking** — Query summaries of all activities including works, funding, and institutional affiliations.
- **Registry Search** — Search the global ORCID database using Solr syntax to find researchers by name, email, or keywords.
- **Item Management** — Deep dive into specific works or funding items using unique put-codes to retrieve full metadata.
- **Member API Features** — For authorized users, create, update, or delete items within sections to keep researcher profiles synchronized.

### How it works

1. Subscribe to this server
2. Enter your ORCID Access Token (Public or Member API)
3. Start querying academic records from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Academic Researchers** — quickly verify profile data and manage your own publication list without manual entry
- **University Administrators** — automate the retrieval of faculty activities and affiliations for reporting
- **Data Scientists** — search and analyze researcher metadata for bibliometric studies and mapping scientific networks


## Available Tools (13)
- **delete_item**: Requires Member API access.

Delete an item from a section (Member API only)
- **expanded_search**: Search the ORCID registry and return expanded metadata
- **get_activities**: Get summary of all activities for an ORCID record
- **get_item**: Get a specific item from a section using its put-code
- **get_person**: Get biographical section of an ORCID record
- **get_record**: Get summary view of the full ORCID record
- **get_section**: Get summary of a specific section
- **get_summary**: Requires Member API access.

Get validated and self-asserted summary (Member API only)
- **register_webhook**: Requires Premium Member API.

Register a webhook callback URL for an ORCID record (Premium only)
- **search**: Supports fields like given-names, family-name, email, orcid, etc.

Search the ORCID registry using Solr 3.6 syntax
- **update_item**: Requires Member API access.

Update an existing item in a section (Member API only)
- **create_item**: Requires Member API access and appropriate scopes.

Add a new item to a section (Member API only)
- **csv_search**: Search the ORCID registry and return CSV format


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ORCID** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search the ORCID registry for researchers with the family name 'Einstein'."

**🤖 AI Agent:**
> I've searched the registry. I found several records, including 'Albert Einstein' (ORCID: 0000-0001-XXXX-XXXX). Would you like me to fetch the full record summary for this iD?

---

**👤 You:**
> "Get the biographical details for ORCID iD 0000-0002-1825-0097."

**🤖 AI Agent:**
> Fetching biographical data using `get_person`... The record belongs to Josiah Carberry. It includes verified names, associated email addresses, and a list of other identifiers like Scopus Author ID.

---

**👤 You:**
> "List all the works associated with ORCID 0000-0002-1825-0097."

**🤖 AI Agent:**
> I've retrieved the 'works' section. There are 12 items listed. Notable titles include 'Toward a Unified Theory of High-Energy Metrology'. Would you like the full details for any specific work?


## ❓ FAQ

**Q: Can I search for researchers by their name or email address?**
Yes! Use the `search` tool with Solr syntax (e.g., `family-name:Smith` or `email:user@example.com`) to find matching records in the ORCID registry.

**Q: How do I retrieve the full details of a specific publication?**
First, use `get_section` with the section 'works' to find the item's `put_code`. Then, use the `get_item` tool with that code to fetch the complete metadata for that specific work.

**Q: Do I need a Member API account to add or update records?**
Yes. While reading public data works with the Public API, tools like `create_item`, `update_item`, and `delete_item` require Member API access and the `useMemberApi` configuration set to true.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/orcid](https://vinkius.com/mcp/orcid)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ORCID** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `orcid` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ORCID** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "orcid": {
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
