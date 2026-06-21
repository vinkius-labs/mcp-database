# Europeana MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/europeana)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Explore millions of cultural heritage items — search artworks, books, and records from European museums and libraries directly through your AI agent.

## Description
Connect to **Europeana**, the digital heart of Europe's cultural heritage. This MCP server allows your AI agent to search and retrieve metadata for millions of digitized items from thousands of European galleries, libraries, archives, and museums.

### What you can do

- **Advanced Search** — Use `search_records` to find specific items using boolean operators and filters (e.g., searching for 'Paris' AND 'Louvre' with image filters).
- **Detailed Metadata** — Retrieve deep technical and descriptive metadata for specific cultural objects using `get_record` with collection and record IDs.
- **Entity Exploration** — Discover linked information about People, Places, Topics, and Organizations associated with cultural records via `get_entity`.
- **Bulk Harvesting** — Access professional-grade metadata harvesting through the `oaipmh_request` tool for large-scale data analysis.

### How it works

1. Subscribe to this server
2. Enter your Europeana API Key (WSKey)
3. Start exploring European history and art from Claude, Cursor, or any MCP client

### Who is this for?

- **Researchers & Academics** — Quickly find primary sources and metadata for historical research.
- **Educators** — Discover high-quality cultural assets and descriptions for lesson planning.
- **Developers & Data Scientists** — Access structured cultural data for applications or analysis via OAI-PMH.


## Available Tools
- **get_entity**: Retrieve information about linked entities
- **oaipmh_request**: Returns XML data.

Bulk harvesting of metadata via OAI-PMH
- **get_record**: Get detailed information about a specific cultural heritage object
- **search_records**: Search Europeana metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Europeana** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search Europeana for records related to 'Vermeer' and 'Delft'."

**🤖 AI Agent:**
> I found several records. Notable items include 'View of Delft' and 'The Little Street'. Would you like the detailed metadata for any of these specific records?

---

**👤 You:**
> "Get the full record details for collection 9200365 and record BibliographicResource_1000055440343."

**🤖 AI Agent:**
> Fetching record details... This is a bibliographic resource from the National Library of France. It includes descriptions in multiple languages and links to the digital object. Would you like to see the full metadata profile?

---

**👤 You:**
> "Retrieve information about the entity 'Leonardo da Vinci' using the entity tool."

**🤖 AI Agent:**
> I've retrieved the entity data for Leonardo da Vinci. It includes his biographical dates, professional roles (painter, engineer, scientist), and links to related records in the Europeana database.


## ❓ FAQ

**Q: How can I filter my search to only include images?**
You can use the `qf` (Query Filter) parameter in the `search_records` tool. For example, setting `qf=TYPE:IMAGE` will narrow your results to visual media only.

**Q: Can I retrieve information about a specific artist or historical figure?**
Yes! Use the `get_entity` tool with the type set to 'person' and the corresponding entity ID to fetch detailed information about individuals linked to Europeana records.

**Q: What is the OAI-PMH tool used for?**
The `oaipmh_request` tool is designed for bulk harvesting of metadata. It allows you to list identifiers, sets, and records in XML format, which is ideal for large-scale data integration and archival synchronization.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/europeana](https://vinkius.com/mcp/europeana)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Europeana** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `europeana` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Europeana** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "europeana": {
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
