# Regulations.gov (eRulemaking) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/regulationsgov-erulemaking)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Access US federal regulations, search documents, public comments, and dockets directly from agencies like the EPA and FAA.

## Description
Connect your AI agent to the **Regulations.gov** database to navigate the US federal rulemaking process with ease. This server provides direct access to the eRulemaking Program, allowing you to monitor legislative changes and public discourse across hundreds of federal agencies.

### What you can do

- **Document Search** — Find rules, proposed rules, and notices using keywords, agency IDs, or specific posting dates.
- **Public Comments** — Retrieve and analyze public feedback submitted to federal agencies to understand community sentiment on specific regulations.
- **Docket Tracking** — Access complete docket folders containing all supporting materials and related documents for specific rulemaking actions.
- **Deep Metadata** — Fetch detailed information about document types, comment periods, and modification histories to stay ahead of regulatory deadlines.

### How it works

1. Subscribe to this server
2. Enter your Regulations.gov API Key
3. Start querying federal data from Claude, Cursor, or any MCP-compatible client

Stay informed about government transparency and regulatory updates without manually browsing complex government portals. Your AI acts as a specialized regulatory analyst.


## Available Tools (6)
- **get_document**: Get details for a specific document
- **search_comments**: Search public comments
- **get_comment**: Get details for a specific comment
- **get_docket**: Get details for a specific docket
- **search_dockets**: Search dockets
- **search_documents**: Search for documents (rules, notices, etc.)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Regulations.gov (eRulemaking)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for recent documents from the EPA related to 'air quality' posted after 2024-01-01."

**🤖 AI Agent:**
> I've found several documents from the EPA regarding air quality. The most recent is a Proposed Rule (ID: EPA-HQ-OAR-2023-0014) regarding emission standards. Would you like to see the full details or the associated comments?

---

**👤 You:**
> "Find public comments submitted for document ID FAA-2023-1234-0001."

**🤖 AI Agent:**
> I've retrieved 15 public comments for that FAA document. They range from industry feedback to individual pilot concerns. I can summarize the top comments or fetch the full text of a specific one for you.

---

**👤 You:**
> "Get the full details for docket folder CMS-2024-0005."

**🤖 AI Agent:**
> Accessing docket CMS-2024-0005... This docket is managed by the Centers for Medicare & Medicaid Services and contains 3 supporting documents and 1 final rule. The last modification was on 2024-02-15.


## ❓ FAQ

**Q: How can I filter documents by a specific government agency?**
Use the `search_documents` tool and provide the `agencyId` parameter (e.g., 'EPA', 'FAA', or 'CMS'). This will restrict the results to materials published only by that specific agency.

**Q: Is it possible to see what the public is saying about a specific rule?**
Yes! Use the `search_comments` tool with the `commentOnId` parameter set to the unique Document ID. You can then use `get_comment` with a specific Comment ID to read the full text of any submission.

**Q: How do I get the complete history of a specific rulemaking folder?**
Use the `get_docket` tool with the specific Docket ID. This retrieves the primary metadata for the docket, while `search_documents` with the same docket ID can list all associated rules and supporting materials.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/regulationsgov-erulemaking](https://vinkius.com/mcp/regulationsgov-erulemaking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Regulations.gov (eRulemaking)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `regulationsgov-erulemaking` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Regulations.gov (eRulemaking)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "regulationsgov-erulemaking": {
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
