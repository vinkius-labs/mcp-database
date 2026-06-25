# ORCID (Researcher IDs) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/orcid-researcher-ids)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Connect to the ORCID registry to search for researchers, fetch biographical data, and manage research activities like works and funding.

## Description
Connect the **ORCID** registry to your AI agent to seamlessly navigate the global ecosystem of researcher identifiers and scholarly records.

### What you can do

- **Registry Search** — Perform standard or expanded Solr searches to find researchers by name, institution, or keywords using `search` and `expanded_search`.
- **Profile Summaries** — Retrieve complete researcher records, including biographical details and activity summaries, via `get_record` and `get_activities`.
- **Works & Funding** — Inspect specific research outputs and funding history using `get_works` or drill down into specific items with `get_section_item`.
- **Trust Markers** — Access validated trust markers for records using `get_summary` (requires Member API).
- **Record Management** — Add or update items in an ORCID record directly through the agent using `add_item` and `update_item` (requires Member API).

### How it works

1. Subscribe to this server
2. Enter your ORCID Access Token (Public or Member API)
3. Start querying researcher data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Academic Researchers** — quickly find collaborators and verify publication records without manual searching
- **Librarians & Data Managers** — automate the retrieval of institutional research outputs and metadata
- **Grant Officers** — verify researcher credentials and funding history directly within your workflow


## Available Tools (14)
- **get_works**: Get summary of research works for an ORCID record
- **register_webhook**: Requires /webhook scope.

Register a webhook for an ORCID record (Premium Member API only)
- **search**: Search the ORCID registry (Standard)
- **unregister_webhook**: Unregister a webhook for an ORCID record (Premium Member API only)
- **update_item**: Requires Member API access token.

Update an existing item in an ORCID record (Member API only)
- **add_item**: Requires Member API access token with /activities/update or /person/update scope.

Add a new item to an ORCID record (Member API only)
- **delete_item**: Requires Member API access token.

Delete an item from an ORCID record (Member API only)
- **expanded_search**: Search the ORCID registry (Expanded)
- **get_activities**: Get summary of all activities for an ORCID record
- **get_person**: Get biographical section of an ORCID record
- **get_record**: Get full summary of an ORCID record
- **get_section_item**: Get full details for a specific item in an ORCID record
- **get_summary**: Requires Member API access token.

Get validated trust markers (Member API only)
- **csv_search**: Search the ORCID registry and return CSV data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ORCID (Researcher IDs)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search the ORCID registry for researchers with the family name 'Einstein'."

**🤖 AI Agent:**
> I've searched the registry. I found several records for 'Einstein'. The most prominent is Albert Einstein (ORCID: 0000-0001-5109-3700). Would you like to see his full record summary?

---

**👤 You:**
> "Get the biographical details for ORCID 0000-0002-1825-0097."

**🤖 AI Agent:**
> Retrieving biographical data... For ORCID 0000-0002-1825-0097, the researcher is Josiah Carberry. He is affiliated with Brown University and his research focuses on psychoceramics. Would you like to see his list of works?

---

**👤 You:**
> "List all research works for ORCID 0000-0003-1415-9265."

**🤖 AI Agent:**
> Fetching works summary... I found 12 research works for this ORCID iD. Notable titles include 'Advanced Quantum Computing' and 'Neural Network Optimization'. Would you like the full details for any of these using their put-code?


## ❓ FAQ

**Q: Can I search for researchers by their institution or specific keywords?**
Yes! Use the `expanded_search` tool with a Solr query like `affiliation-name:"University of Oxford"` to find researchers associated with specific organizations along with their profile details.

**Q: How do I retrieve the full list of publications for a specific ORCID iD?**
You can use the `get_works` tool by providing the researcher's ORCID iD. This will return a summary of all research works associated with that record.

**Q: Is it possible to add new research items to an ORCID profile using this server?**
Yes, if you have a Member API access token with the appropriate scopes, you can use the `add_item` tool to add works, funding, or other activities to a record.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/orcid-researcher-ids](https://vinkius.com/mcp/orcid-researcher-ids)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ORCID (Researcher IDs)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `orcid-researcher-ids` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ORCID (Researcher IDs)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "orcid-researcher-ids": {
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
