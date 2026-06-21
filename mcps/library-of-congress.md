# Library of Congress MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/library-of-congress)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Search and retrieve millions of historical items, maps, photos, and manuscripts from the world's largest library.

## Description
Connect your AI agent to the **Library of Congress** (LOC) and explore the vast digital archives of the United States' oldest federal cultural institution. Access millions of records, from historical newspapers to rare maps and sound recordings.

### What you can do

- **Global Search** — Search across the entire LOC catalog including items, legislation, and blogs using the `search` tool.
- **Digital Collections** — Browse and list all available digital collections or drill down into specific ones like the 'Abraham Lincoln Papers' using `list_collections` and `get_collection_items`.
- **Format-Specific Discovery** — Filter your research by specific media types such as maps, audio, or photos with `search_format`.
- **Deep Bibliographic Research** — Retrieve detailed metadata and digital resource links for specific items using `get_item`.
- **OCR & Text Analysis** — Access full-text OCR, word coordinates, and context snippets for digitized documents via `get_text_service`.
- **Technical Image Metadata** — Fetch IIIF technical data for high-resolution images using `get_image_info`.

### How it works

1. Subscribe to this server
2. Enter your Library of Congress API Key (optional but recommended for higher rate limits)
3. Start researching historical data directly from your MCP-compatible client

### Who is this for?

- **Researchers & Historians** — Instantly find primary sources and bibliographic data without manual catalog navigation.
- **Educators & Students** — Access digitized manuscripts and historical records for curriculum development.
- **Data Scientists** — Utilize OCR services and metadata for large-scale historical text analysis.


## Available Tools
- **get_collection_items**: List items within a specific collection
- **list_collections**: List all digital collections
- **search_format**: g., maps, photos, audio).

Search items of a specific format
- **get_image_info**: json for a specific image identifier.

Get technical metadata about an image (IIIF)
- **get_item**: Get detailed bibliographic data for a single item
- **get_resource**: g., a specific page of a newspaper) using resource_id.

Get access to discrete digitized files
- **search**: using a keyword query.

Search the entire Library of Congress website
- **get_text_service**: Access full-text OCR, word coordinates, and context snippets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Library of Congress** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search the Library of Congress for Civil War maps of Virginia."

**🤖 AI Agent:**
> I've found several maps. Notable items include 'Map of the seat of war in Virginia' (1861) and 'Central Virginia: showing Lieut. Gen'l. U.S. Grant's campaign'. Would you like the bibliographic details for any of these?

---

**👤 You:**
> "List all items in the 'world-war-i-posters' collection."

**🤖 AI Agent:**
> Retrieving items from the World War I Posters collection... I've found items like 'I want you for U.S. Army' and 'Destroy this mad brute'. There are 25 items on the first page. Should I fetch more or get details for a specific poster?

---

**👤 You:**
> "Get the full text for the document segment 'service/gdc/gdcscd/00/01/02/03/0001.txt'."

**🤖 AI Agent:**
> Accessing text services... I have retrieved the full OCR transcript for that segment. It begins with: 'PROCEEDINGS OF THE CONVENTION...'. Would you like me to summarize the content or search for a specific term within it?


## ❓ FAQ

**Q: Can I search for items specifically in a format like 'maps' or 'audio'?**
Yes! Use the `search_format` tool and specify the format parameter (e.g., 'maps', 'photos', 'audio') along with your query to get targeted results.

**Q: How do I get the full OCR text of a digitized document?**
You can use the `get_text_service` tool. Provide the document segment path and set the `full_text` parameter to 1 to retrieve the complete OCR transcript.

**Q: Can I list items from a specific collection like the Abraham Lincoln papers?**
Yes. Use the `get_collection_items` tool with the collection slug (e.g., 'abraham-lincoln-papers') to see all items contained within that specific archive.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/library-of-congress](https://vinkius.com/mcp/library-of-congress)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Library of Congress** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `library-of-congress` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Library of Congress** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "library-of-congress": {
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
