# GovInfo (GPO Legislative Docs) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/govinfo-gpo-legislative-docs)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Access official US government documents, legislative bills, and federal registers directly from the GPO.

## Description
Connect your AI agent to the **GovInfo** API by the U.S. Government Publishing Office (GPO) to research and retrieve official federal documents through natural conversation.

### What you can do

- **Explore Collections** — List all available document categories like Congressional Bills, the Federal Register, and Presidential Papers
- **Advanced Search** — Use Lucene syntax to perform complex queries across the entire GPO database for specific keywords or topics
- **Document Retrieval** — Fetch detailed metadata, summaries, and historical context for specific legislative packages
- **Content Access** — Retrieve document content in multiple formats including PDF, XML, and MODS for deep analysis
- **Date-based Filtering** — Track legislative changes and new publications by listing packages within specific timeframes

### How it works

1. Subscribe to this server
2. Enter your GovInfo (Data.gov) API Key
3. Start querying official government data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal Professionals** — quickly find specific bill versions, federal regulations, or court opinions without manual portal navigation
- **Researchers & Journalists** — track government activity, historical records, and policy changes using automated queries
- **Policy Analysts** — monitor legislative progress and federal notices in real-time to stay ahead of regulatory shifts


## Available Tools
- **get_collection_details**: Get metadata for a specific GovInfo collection
- **get_package_content**: Note: Binary formats like pdf or zip will be returned as raw text/binary strings.

Download or retrieve GovInfo package content
- **get_package_summary**: Get detailed metadata for a specific GovInfo package
- **list_collections**: g., Congressional Bills, Federal Register).

List all available GovInfo document collections
- **list_packages**: List packages within a GovInfo collection by date
- **search_govinfo**: Search GovInfo collections


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GovInfo (GPO Legislative Docs)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available GovInfo document collections."

**🤖 AI Agent:**
> I've retrieved the available collections. You can access documents from the Federal Register (FR), Congressional Bills (BILLS), Daily Compilation of Presidential Documents (DCPD), and many others. Which collection would you like to explore?

---

**👤 You:**
> "Search for recent Congressional Bills related to 'artificial intelligence'."

**🤖 AI Agent:**
> Searching the database... I found several recent bills, including 'H.R. 3849' and 'S. 1624'. Would you like me to fetch the summary for one of these specific packages?

---

**👤 You:**
> "Get the summary and metadata for package ID BILLS-117hr3076ih."

**🤖 AI Agent:**
> Here is the summary for H.R. 3076 (Postal Service Reform Act of 2022). It was introduced in the 117th Congress and focuses on the financial stability of the USPS. I have also retrieved the MODS and XML metadata links if you need further details.


## ❓ FAQ

**Q: Can I search for specific keywords across all government documents?**
Yes! Use the `search_govinfo` tool with Lucene syntax to perform complex queries. You can filter by date, collection, or specific fields to find exactly what you need.

**Q: How do I get the actual text or PDF of a bill?**
Use the `get_package_content` tool with the specific `packageId` and choose your preferred format (pdf, xml, mods, etc.) to retrieve the document content.

**Q: What types of document collections are available?**
Run the `list_collections` tool to see all available sources. Common codes include 'BILLS' for Congressional Bills, 'FR' for the Federal Register, and 'CPD' for Compilation of Presidential Documents.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/govinfo-gpo-legislative-docs](https://vinkius.com/mcp/govinfo-gpo-legislative-docs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GovInfo (GPO Legislative Docs)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `govinfo-gpo-legislative-docs` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GovInfo (GPO Legislative Docs)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "govinfo-gpo-legislative-docs": {
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
