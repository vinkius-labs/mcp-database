# Federal Register API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/federal-register-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access US public documents — audit rules and agencies via AI.

## Description
Empower your AI agent to orchestrate your entire public policy research and document auditing workflow with the **Federal Register API**, the authoritative source for United States government rules and notices. By connecting the Federal Register to your agent, you transform complex administrative searches into a natural conversation. Your agent can instantly retrieve active document details, audit agency publications, and query specific rule metadata without you ever touching a government portal. Whether you are conducting regulatory research or managing regional policy constraints, your agent acts as a real-time administrative consultant, ensuring your data is always verified and precise.

### What you can do

- **Document Auditing** — Search for thousands of public documents and rules by keyword and retrieve detailed metadata, including publication dates and agencies.
- **Agency Oversight** — Audit all US government agencies that publish in the Federal Register to understand the administrative reach of public sector rules instantly.
- **Rule Discovery** — Query specific document numbers to assist in deep-dive regulatory and temporal classification.
- **Metadata Intelligence** — Retrieve unique document identifiers and HTML links to assist in professional policy auditing.
- **Operational Monitoring** — Check API status to ensure your document research workflow is always operational.

### How it works

1. Subscribe to this server
2. No API Key required (Federal Register is a free and open service)
3. Start managing your administrative intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Policy Analysts & Journalists** — monitor government notices and retrieve official metadata straight from your workflow.
- **Legal Researchers** — verify public rules and audit agency patterns without manual searching.
- **Regulatory Leads** — perform rapid audits of administrative markers and identify relevant policy patterns through natural language.
- **Operations Leads** — automate government data querying to orchestrate cross-functional outreach teams smoothly.


## Available Tools (4)
- **check_api_status**: Check if the Federal Register service is operational
- **get_federal_document_details**: Get full metadata and HTML links for a specific federal document
- **list_federal_agencies**: List all government agencies that publish in the Federal Register
- **search_federal_documents**: Search for public documents and rules in the Federal Register


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Federal Register API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for documents about 'environmental protection' in the Federal Register."

**🤖 AI Agent:**
> I've retrieved several documents about environmental protection! Notable entries include rules from the EPA and notices regarding new sustainability standards. Would you like the full details for the top matches or the agency metadata?

---

**👤 You:**
> "Show details for Federal Register document '2023-00001'."

**🤖 AI Agent:**
> I've retrieved the details for document 2023-00001! It is titled [Title] and was published by [Agency]. I can provide the official link to the full text and the publication date metadata for you.

---

**👤 You:**
> "List all agencies that publish in the Federal Register."

**🤖 AI Agent:**
> I've scanned the agency catalog! There are hundreds of federal entities listed, including the EPA, Department of Energy, and the FDA. I can help you search for specific documents from any of these thematic clusters.


## ❓ FAQ

**Q: Is an API Key required for Federal Register API?**
No. The Federal Register API is a free and open service provided by the United States government. This server works out of the box without any static credentials required.

**Q: What types of documents are available?**
The API provides access to rules, proposed rules, notices, and presidential documents published in the Federal Register.

**Q: Can the agent show agency publication counts?**
Yes. The `list_federal_agencies` tool retrieves the list of agencies along with their metadata, assisting in identifying which entities publish most frequently.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/federal-register-api](https://vinkius.com/mcp/federal-register-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Federal Register API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `federal-register-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Federal Register API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "federal-register-api": {
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
