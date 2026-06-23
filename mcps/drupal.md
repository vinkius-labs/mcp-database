# Drupal MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/drupal)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage headless content via Drupal — list nodes, handle taxonomy terms, manage files, and audit users directly from any AI agent.

## Description
Connect your **Drupal** site to any AI agent and take full control of your headless content management and JSON:API workflows through natural conversation.

### What you can do

- **Content Node Orchestration** — Identify bounded routing spaces inside headless Drupal models and extract explicitly attached REST arrays tracking standard JSON:API boundaries
- **Entity Management** — Provision highly-available JSON payloads to write rows into Drupal entities, or irreversibly vaporize nodes to clear live document entities
- **Revision Mutation** — Substitute draft values safely by triggering HTTP PATCH operations to replace row segments isolating partial updates mapping specific UUIDs
- **Taxonomy Management** — Enumerate explicitly attached structured rules defining how content is categorized natively through terms and vocabularies
- **File & Media Discovery** — Taps raw configurations pulling explicitly managed Drupal files to discover raw CDN URIs mitigating headless media blocking
- **Identity Oversight** — Evaluate physical arrays isolating actual editors and administrators exposing their metadata and access roles securely
- **Metadata Auditing** — Retrieve the exact structural matching verifying file storage and analyzing explicit UUID bounds for managed attachments

### How it works

1. Subscribe to this server
2. Enter your Drupal Base URL and Auth Header (e.g., 'Basic Base64-Credentials'). Ensure the JSON:API module is enabled on your site.
3. Start managing your headless content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Managers & Editors** — create and update content nodes and manage taxonomy terms without the Drupal admin UI
- **Full-stack Developers** — test and debug JSON:API endpoints and verify entity schemas directly from the IDE
- **Digital Marketers** — manage media assets and categorize content using natural language conversation
- **Ops Teams** — audit registered users and monitor managed file storage in real-time


## Available Tools (10)
- **create_cms_node**: Provision a highly-available JSON Payload writing Rows into Drupal entities
- **wipe_cms_node**: Irreversibly vaporize explicit App nodes dropping live Document entities
- **get_file_metadata**: Retrieve the exact structural matching verifying File storage
- **get_single_node**: Retrieve explicit Cloud logging tracing explicit Node UUIDs
- **get_taxonomy_term**: Perform structural extraction of properties driving active Term mappings
- **list_managed_files**: Inspect deep internal arrays mitigating specific Picture constraints
- **list_content_nodes**: Identify bounded routing spaces inside the Headless Drupal models
- **list_term_vocabularies**: Enumerate explicitly attached structured rules exporting Taxonomies
- **list_drupal_users**: Identify precise active arrays spanning rented Admin identities
- **patch_cms_node**: Mutate global Web CRM boundaries substituting Draft values safely


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Drupal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 'article' nodes from Drupal"

**🤖 AI Agent:**
> Retrieving articles... I found 5 recent nodes including 'Welcome to Headless Drupal' (UUID: 123) and 'JSON:API Basics' (UUID: 456). Would you like me to fetch the full content for any of these?

---

**👤 You:**
> "Create an 'article' with title 'AI Integration' and body 'Testing Drupal MCP...'"

**🤖 AI Agent:**
> Node created successfully! Your new article 'AI Integration' has been persisted in Drupal with UUID: 'abc-789'. You can now view it in your frontend or admin UI.

---

**👤 You:**
> "Show me all terms in the 'tags' vocabulary"

**🤖 AI Agent:**
> Retrieving tags... I found 10 registered terms including 'Technology', 'Tutorial', 'Drupal', and 'API'. Would you like the metadata for a specific tag?


## ❓ FAQ

**Q: Can my agent create a new content node in Drupal?**
Yes. Use the 'create_cms_node' tool. Provide the node type (e.g., 'article') and a JSON object with the attributes. The agent will orchestrate the HTTP POST request to your Drupal JSON:API to persist the entity.

**Q: How do I list all taxonomy terms for a specific vocabulary?**
Use the 'list_term_vocabularies' tool. Provide the vocabulary ID (e.g., 'tags'). Your agent will execute bulk iterations to track explicitly registered terms and return them within your chat context.

**Q: Can I retrieve the direct URL for a managed image file?**
Absolutely. Use the 'get_file_metadata' tool with the file ID. The agent will analyze the explicit UUID bounds and fetch the literal URL parameters, providing the public location of the managed attachment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/drupal](https://vinkius.com/mcp/drupal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Drupal** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `drupal` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Drupal** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "drupal": {
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
