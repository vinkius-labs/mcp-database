# Collection Catalog Deduplicator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/collection-catalog-deduplicator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Identifies and merges duplicate collection records using identifiers and descriptive attributes.

## Description
This MCP server provides essential tools for maintaining data integrity in collections. It allows AI agents to identify duplicate entries by matching identifiers like ISBN or UPC, or by comparing titles and editions. Use `find_duplicates` to group identical items, `merge_records` to create a single master record from duplicates, and `calculate_catalog_integrity` to assess the health of your collection.


## Available Tools (4)
- **find_duplicates**: Identifies groups of records that represent the same item based on matching criteria
- **calculate_catalog_integrity**: Provides a statistical overview of the collection's health
- **filter_by_owner**: Isolates all records belonging to a specific person
- **merge_records**: Collapses a specific group of duplicate records into a single, high-fidelity master record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Collection Catalog Deduplicator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all duplicate records in this list: [{'id': '1', 'title': 'The Great Gatsby', 'edition': '1st', 'identifier': '12345'}, {'id': '2', 'title': 'The Great Gatsby', 'edition': '1st', 'identifier': '12345'}]"

**🤖 AI Agent:**
> I found 1 group of duplicates containing 2 records.

---

**👤 You:**
> "What is the integrity report for my collection?"

**🤖 AI Agent:**
> Your collection has 100 total entries, 5 duplicates, and 95 unique items, resulting in a duplicate ratio of 0.05.

---

**👤 You:**
> "Show me all items owned by Alice."

**🤖 AI Agent:**
> Alice owns 3 items: 'Vintage Camera', 'Leather Journal', and 'Fountain Pen'.


## ❓ FAQ

**Q: How does the tool identify duplicates?**
The `find_duplicates` tool identifies matches if the identifier (like an ISBN) is identical, or if both the title and edition match exactly when no identifier is present.

**Q: Can I merge multiple records into one?**
Yes, you can use `merge_records` to collapse a group of duplicate IDs into a single master record that preserves the most complete metadata.

**Q: How can I check the health of my collection?**
You can use `calculate_catalog_integrity` to get a statistical report including total entries, duplicate counts, and the duplicate ratio.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/collection-catalog-deduplicator](https://vinkius.com/en/ai-agent-connect/collection-catalog-deduplicator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Collection Catalog Deduplicator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `collection-catalog-deduplicator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Collection Catalog Deduplicator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "collection-catalog-deduplicator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
