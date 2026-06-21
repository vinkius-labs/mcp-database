# Figshare MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/figshare)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Manage research data and scholarly outputs via Figshare — list public articles, manage private uploads, and organize collections directly from your AI agent.

## Description
Connect your **Figshare** account to any AI agent to streamline your research data management and publication workflows through natural conversation.

### What you can do

- **Article Management** — List public articles, fetch specific article details, and create, update, or delete private articles in your account.
- **File Handling** — List files associated with articles, initiate multi-part S3 uploads, and track file details for your research datasets.
- **Collections & Projects** — Create and list public collections and projects to organize your scholarly output effectively.
- **Metadata Control** — Update titles, descriptions, and other metadata for your articles to ensure they are discoverable and well-documented.

### How it works

1. Subscribe to this server
2. Enter your Figshare Personal Access Token
3. Start managing your research repository from Claude, Cursor, or any MCP-compatible client

No more manual navigation through repository interfaces to check upload statuses or update metadata. Your AI acts as a research data manager.

### Who is this for?

- **Researchers & Academics** — quickly upload datasets, update article descriptions, and check publication statuses without leaving your workspace.
- **Data Managers** — automate the organization of large collections and projects across institutional repositories.
- **Librarians & Archivists** — query public research outputs and manage metadata updates efficiently.


## Available Tools
- **complete_file_upload**: Complete a file upload
- **create_collection**: Create a new collection
- **create_private_article**: Create a new private article
- **create_project**: Create a new project
- **delete_article**: Delete an article
- **get_article_downloads**: Get total downloads for an article
- **get_article**: Get details of a specific article
- **get_article_views**: Get total views for an article
- **get_custom_fields**: Get custom metadata fields for the institution
- **get_file_details**: Get file details
- **get_hrfeed_upload**: Get HR feed upload details
- **initiate_file_upload**: Initiate a file upload for an article
- **list_article_files**: List files for an article
- **list_public_articles**: List public articles
- **list_public_collections**: List public collections
- **list_public_projects**: List public projects
- **search_articles**: Advanced search for articles
- **search_collections**: Advanced search for collections
- **search_projects**: Advanced search for projects
- **update_article**: Update an existing article


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Figshare** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recent public articles on Figshare."

**🤖 AI Agent:**
> I've retrieved the latest public articles. I found several entries including 'Climate Change Impact on Alpine Flora' and 'Dataset for Neural Network Optimization'. Would you like details on any of these?

---

**👤 You:**
> "Create a private article titled 'Lab Results Q4' with the description 'Raw data from the December experiments'."

**🤖 AI Agent:**
> Success! I've created the private article 'Lab Results Q4' (ID: 9876543). You can now start uploading files to this draft using the initiate upload tool.

---

**👤 You:**
> "Show me all files attached to article 1234567."

**🤖 AI Agent:**
> Checking files for article 1234567... I found 3 files: 'methodology.pdf', 'raw_data.csv', and 'analysis_script.py'. Would you like the specific details or download URLs for any of these?


## ❓ FAQ

**Q: Can I upload files to a Figshare article using this integration?**
Yes. You can use `initiate_file_upload` to start the process and `complete_file_upload` once the data transfer is finished. You can also use `list_article_files` to verify the contents of any article.

**Q: How do I create a new private draft for my research?**
Simply ask the agent to use the `create_private_article` tool. Provide a title and an optional description, and the agent will generate a new private entry in your Figshare account.

**Q: Is it possible to organize my articles into projects or collections?**
Absolutely. You can use `create_project` or `create_collection` to set up organizational structures, and use `list_public_projects` or `list_public_collections` to browse existing ones.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/figshare](https://vinkius.com/mcp/figshare)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Figshare** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `figshare` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Figshare** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "figshare": {
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
