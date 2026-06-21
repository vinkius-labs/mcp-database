# Campinas Open Data MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/campinas-open-data-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access public data from Campinas, Brazil — search datasets, resources, and city organizations directly from your AI agent.

## Description
Connect to the **Campinas Open Data Portal** (CKAN) and explore a wealth of public information from one of Brazil's major cities through natural conversation.

### What you can do

- **Dataset Discovery** — Search for specific packages related to health, education, finance, or transport using keywords.
- **Metadata Inspection** — Retrieve full metadata for datasets and individual resources (files) to understand data structures.
- **Organizational Mapping** — List all city departments and organizations that provide public data.
- **Thematic Exploration** — Browse data by groups (e.g., 'Saúde', 'Educação') or tags to find relevant information quickly.
- **Resource Access** — Get direct links and metadata for CSVs, PDFs, and APIs hosted on the portal.

### How it works

1. Subscribe to this server
2. Enter your Campinas Portal API Key (optional for public data, required for restricted access)
3. Start querying city data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Academics** — quickly find datasets for urban studies or public policy analysis.
- **Developers** — inspect API resources and data schemas without leaving the code editor.
- **Journalists & Citizens** — explore public spending and city metrics through simple questions.


## Available Tools
- **campinas_list_groups**: g., Education, Health).

List thematic groups
- **campinas_list_organizations**: List organizations providing data
- **campinas_list_packages**: List all dataset names
- **campinas_search_packages**: Search for datasets matching specific criteria
- **campinas_get_package**: Get full metadata for a specific dataset
- **campinas_search_resources**: g., name:financeiro).

Search for resources based on fields
- **campinas_get_resource**: Get metadata for a specific resource
- **campinas_list_tags**: List all tags used across the portal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Campinas Open Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for datasets about 'educação' in Campinas."

**🤖 AI Agent:**
> I found several datasets related to education, including 'Vagas em Creches' and 'Escolas Municipais'. Which one would you like to explore?

---

**👤 You:**
> "List all organizations that provide data to the portal."

**🤖 AI Agent:**
> I've retrieved the list of organizations. There are 25 entities, including the 'Secretaria Municipal de Saúde' and 'Secretaria de Finanças'.

---

**👤 You:**
> "Get full metadata for the dataset 'vagas-em-creches'."

**🤖 AI Agent:**
> Fetching metadata for 'vagas-em-creches'... This dataset includes 3 resources (CSV and PDF) and was last updated on June 2023. It covers nursery school availability by region.


## ❓ FAQ

**Q: How can I search for datasets related to a specific topic like 'Health'?**
You can use the `search_packages` tool with a query string. For example, searching for 'saude' will return all datasets categorized under health in the Campinas portal.

**Q: Can I see which city departments are publishing data?**
Yes! Use the `list_organizations` tool to get a complete list of all city departments and entities that contribute to the Open Data Portal.

**Q: How do I get the download link for a specific data file?**
Use the `get_resource` tool with the specific Resource ID. It will return the metadata, including the URL to download the file (CSV, PDF, etc.).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/campinas-open-data-alternative](https://vinkius.com/mcp/campinas-open-data-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Campinas Open Data** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `campinas-open-data-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Campinas Open Data** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "campinas-open-data-alternative": {
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
