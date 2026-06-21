# Federal Register MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/federal-register)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access the official daily publication for rules, proposed rules, and notices of Federal agencies and organizations.

## Description
Connect your AI agent to the **Federal Register** and navigate the vast landscape of U.S. government regulations and public notices through natural language.

### What you can do

- **Document Search** — Search through millions of documents published since 1994 using filters like agency, date, document type, and RIN.
- **Public Inspection** — Access the 'Public Inspection' desk to see documents scheduled for publication before they officially hit the register.
- **Agency Intelligence** — List all federal agencies and retrieve detailed profiles, including their recent regulatory activity and metadata.
- **Regulatory Tracking** — Monitor specific dockets, Regulation Identifier Numbers (RIN), and CFR titles/parts to stay ahead of compliance changes.
- **Deep Metadata** — Fetch full document details, including publication dates, page ranges, and agency contact information.

### How it works

1. Subscribe to this server
2. No API key is required for standard public access
3. Start querying the Federal Register from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal Professionals** — quickly find specific rules or notices without navigating complex government portals
- **Compliance Officers** — track regulatory changes and public inspection filings in real-time
- **Policy Researchers** — analyze agency activity and historical document trends via AI-driven search


## Available Tools
- **get_agency**: Fetch a single agency by slug
- **get_current_public_inspection**: Retrieve all documents currently on public inspection
- **get_document**: Fetch a single published document
- **get_multiple_documents**: Fetch multiple published documents
- **get_public_inspection_by_date**: Retrieve documents on public inspection on a specific date
- **get_public_inspection_document**: Fetch a single public inspection document
- **list_agencies**: List all federal agencies
- **search_documents**: Search published Federal Register documents
- **search_public_inspection**: Search public inspection documents


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Federal Register** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for recent 'rule' type documents from the Environmental Protection Agency."

**🤖 AI Agent:**
> I've found several recent rules from the EPA. Notable entries include new standards for air quality and water safety. Would you like the full details for any of these document numbers?

---

**👤 You:**
> "What documents are currently on the public inspection desk for today?"

**🤖 AI Agent:**
> I've retrieved the public inspection list for today. There are 15 documents currently filed, including notices from the Department of Energy and the IRS. Should I list the titles and filing times?

---

**👤 You:**
> "Get the profile and recent activity for the agency with slug 'education-department'."

**🤖 AI Agent:**
> I've fetched the details for the Department of Education. They have published 124 documents in the last year. Their profile includes contact info and links to their latest rules. Would you like to see their most recent publication?


## ❓ FAQ

**Q: How do I find documents from a specific agency like the FDA?**
First, use the `list_agencies` tool to find the correct agency slug or ID. Then, use the `search_documents` tool and provide that slug in the `agencies` parameter to filter results.

**Q: Can I see documents before they are officially published in the daily register?**
Yes! Use the `search_public_inspection` or `get_current_public_inspection` tools. These access the 'Public Inspection' desk, which contains documents filed for public review before their formal publication date.

**Q: Is it possible to search for documents related to a specific Regulation Identifier Number (RIN)?**
Absolutely. Use the `search_documents` tool and provide the `rin` parameter. This will return all published documents associated with that specific regulatory action.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/federal-register](https://vinkius.com/mcp/federal-register)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Federal Register** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `federal-register` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Federal Register** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "federal-register": {
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
