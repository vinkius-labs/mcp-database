# DeveloperHub MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/developerhub)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Equip your AI agent to manage documentation projects, track pages, and monitor changelogs via the DeveloperHub API.

## Description
Integrate **DeveloperHub**, the specialized platform for developer documentation, directly into your AI workflow. Manage your documentation portals, monitor page updates and versions, and track product changelogs using natural language.

### What you can do

- **Project Oversight** — List and retrieve technical metadata for all your documentation projects and portals.
- **Page Management** — Access the full page hierarchy, retrieve Markdown content, and track recent updates.
- **Version Control** — Monitor available documentation versions and identify which one is currently active.
- **Changelog Tracking** — List product release notes and updates associated with your documentation projects.

### How it works

1. Connect the DeveloperHub integration to your AI assistant.
2. Authorize using your DeveloperHub API Key (found in your account settings).
3. Orchestrate your developer experience and documentation through intuitive conversation.

### Who is this for?

- **Technical Writers** — Quickly check page statuses and recent modifications on the go.
- **Product Managers** — Monitor changelog entries and documentation readiness during releases.
- **Developer Advocates** — Search for specific documentation snippets and technical details via chat.


## Available Tools (10)
- **get_account_metadata**: Retrieve metadata and usage limits for your DeveloperHub account
- **get_documentation_page_content**: Get the full content and metadata for a specific documentation page
- **get_documentation_sitemap**: Retrieve a structural map of all pages in a project
- **get_documentation_project_details**: Get detailed information for a specific documentation project
- **list_product_changelogs**: List all changelog entries associated with a documentation project
- **list_documentation_pages**: List all pages and sub-pages within a specific project
- **list_documentation_projects**: List all documentation projects in your DeveloperHub account
- **list_recently_updated_pages**: Identify documentation pages that have been recently modified
- **list_documentation_versions**: List all versions (e.g. v1.0, v2.0) available for a project
- **search_documentation_portal**: Search for specific keywords across all pages in a documentation project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DeveloperHub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all documentation pages in the 'API-Reference' project."

**🤖 AI Agent:**
> I've found 15 pages in 'API-Reference', including 'Authentication', 'Endpoints Overview', and 'Error Codes'. Would you like to see the sub-pages for any of these sections?

---

**👤 You:**
> "What were the latest updates in our project changelog?"

**🤖 AI Agent:**
> The latest changelog entries for your project are: 'v2.1.0 - Added GraphQL support', 'v2.0.5 - Improved search performance', and 'v2.0.4 - Bug fixes in SDK'. Should I retrieve the full details for the v2.1.0 update?

---

**👤 You:**
> "Search for 'webhooks' in our documentation portal."

**🤖 AI Agent:**
> I've found 3 pages matching 'webhooks': 'Webhooks Guide', 'Configuring Webhooks', and 'Webhook Events Reference'. Which one would you like to explore?


## ❓ FAQ

**Q: How do I get a DeveloperHub API Key?**
Log in to your DeveloperHub account, navigate to **Project Settings > API**, and you can generate or retrieve your unique API Key from that section.

**Q: Can the agent retrieve the Markdown content of a page?**
Yes, you can use the get_documentation_page_content tool to retrieve the full technical structure and text content of any page in your project.

**Q: Does the integration support searching across portals?**
You can search within a specific project using the search_documentation_portal tool. To search across multiple portals, simply perform separate queries for each project ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/developerhub](https://vinkius.com/mcp/developerhub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DeveloperHub** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `developerhub` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DeveloperHub** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "developerhub": {
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
