# Transifex MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/transifex)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Localize your projects efficiently using AI Agents with the official Transifex integration.

## Description
### What you can do
- **Explore Localization Projects**: Allow your AI agent to list all Transifex projects and track translation progress.
- **Fetch Resources & Strings**: Automatically read your source content directly from Transifex resources.
- **Analyze Supported Languages**: Request your AI to retrieve details of target languages.

### How it works
1. Subscribe to the Transifex MCP integration.
2. Insert your personal Transifex API Token.
3. Enjoy an autonomous AI agent capable of orchestrating your entire localization workflow.

### Who is this for?
- **Developers**: Automate content sync pipelines and debug translation keys.
- **Localization Managers**: Monitor overall project statuses without switching tabs.
- **Product Teams**: Ensure seamless multilingual launches.


## Available Tools
- **get_language**: g., l:en, l:pt_BR).

Get a specific language by ID
- **get_organization**: g., o:org-slug).

Get a specific organization by ID
- **get_project**: g., o:org-slug:p:project-slug).

Get a specific project by ID
- **get_resource_string**: Get a specific resource string by ID
- **get_resource**: g., o:org-slug:p:project-slug:r:resource-slug).

Get a specific resource by ID
- **list_languages**: List supported languages in Transifex
- **list_organizations**: List all organizations the user belongs to
- **list_projects**: Optionally filter by organization ID.

List projects in Transifex
- **list_resource_strings**: This requires the resource ID to filter the strings.

List resource strings (source strings) for a specific resource
- **list_resources**: Optionally filter by project ID.

List resources in Transifex


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Transifex** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Transifex organizations and their projects."

**🤖 AI Agent:**
> I've fetched your Transifex organizations. You currently have access to 1 organization: 'o:my-org'. Here are the projects under this organization...

---

**👤 You:**
> "Get the details for the project with ID 'o:my-org:p:my-project'."

**🤖 AI Agent:**
> Here are the details for the project 'o:my-org:p:my-project'. It is currently active and has 5 resources attached to it.

---

**👤 You:**
> "List all supported languages in Transifex."

**🤖 AI Agent:**
> Transifex supports a wide variety of languages. Here is the list of available language codes and their details...


## ❓ FAQ

**Q: Can the AI agent create new translation strings or modify them?**
Currently, this integration focuses on listing and retrieving localization data (projects, resources, strings, languages) to ensure read-only safety.

**Q: What is the format of the organization and project IDs?**
Transifex uses unique slugs prefixed with identifiers, such as 'o:organization-slug' for organizations and 'o:org-slug:p:project-slug' for projects. Your AI will use these to fetch specific details.

**Q: Does this integration support multiple Transifex organizations?**
Yes, the agent can list and interact with all organizations that your API Token has access to.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/transifex](https://vinkius.com/mcp/transifex)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Transifex** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `transifex` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Transifex** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "transifex": {
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
