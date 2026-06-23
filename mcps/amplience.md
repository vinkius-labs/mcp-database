# Amplience MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amplience)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Connect your Amplience CMS to your AI agent — query hubs, pull content, edit schemas, and deploy live items easily via chat.

## Description
Link your **Amplience** headless CMS to any intelligent AI agent to completely rethink how you handle your enterprise content architecture, deploying components natively through standard conversation.

### What you can do

- **Discover Asset Hierarchies** — Freely list top-level Hubs, target specific Repositories, and fetch internal Folders to help your AI inherently understand where every graphic and article lives.
- **Content Retrieval** — Paginate through dynamic content items, safely extracting complete metadata alongside current active schemas and validation rules.
- **Edit & Create Structure** — Give the agent full permission to push correctly strictly-typed JSON payloads back into the system, generating or modifying blog entries and product metadata.
- **Manage Deployments** — Permanently execute deletions (if revision locks permit) or instruct the system to fire a specific content configuration directly over to the edge delivery API to hit the live website.

### How it works

1. Enable the connector within your environment.
2. Submit your exact Amplience Hub Name alongside a Personal Access Token.
3. Oversee and iterate your site configurations natively using Claude, Cursor, or other MCP counterparts.

### Who is this for?

- **E-commerce Managers** — ask the agent to rapidly locate the Black Friday banner content configuration block and update the live URL paths seamlessly.
- **Frontend Developers** — have your IDE agent read the precise output validation structure of an Amplience schema and automatically scaffold the corresponding React/Vue TypeScript interface in your project.
- **Content Marketers** — command your agent to create a brand new draft for a promotional blog post, pre-populating fields utilizing your CRM's specific SEO guidelines.


## Available Tools (10)
- **create_content_item**: Create a new structured content item adhering to a schema inside a folder
- **delete_content_item**: Requires version validation before deletion.

Permanently delete a content item from the repository database
- **get_content_item**: Retrieve a specific content item configuration and its schema revision lock
- **list_content_items**: Retrieve paginated content items from a specific repository
- **get_delivery_content**: Retrieve the exact structural matching verifying Delivery CDN blocks
- **list_folders**: List all folders organizing content in a given repository
- **list_hubs**: Essential for retrieving the active workspace.

List all accessible Amplience Hubs (environments)
- **list_repositories**: List all content repositories within a specific Hub
- **publish_content_item**: Publish a specific content item version to the live delivery CDN
- **update_content_item**: Update an existing content item data structure matching its current schema


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amplience** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Identify all active repositories present inside my default Amplience Hub."

**🤖 AI Agent:**
> Extracted Repositories:
1. Core Web Components (ID: `6k33i1`)
2. Blog Content (ID: `6m75o9`)
3. Banner Ad Images (ID: `9q82y3`)
Which one would you like me to inspect into its foundational folder paths?

---

**👤 You:**
> "Pull the structural metadata (schema lock and payload) of item '5tYv92'."

**🤖 AI Agent:**
> Here is Content Item '5tYv92' ('Spring Banner 2024'):
Schema Lock Version: 5
Payload: `{ "title": "Spring Sales!", "href": "/shop/spring" }`
If you want to modify this banner output structure, simply provide the changes.

---

**👤 You:**
> "Publish the newly edited Content '5tYv92' to the global live network."

**🤖 AI Agent:**
> Understood. Bypassing draft constraints and hitting publication edge. Content Item '5tYv92' has been published correctly from mapping to live domain! Would you like me to fetch the delivery URL JSON logic for verification?


## ❓ FAQ

**Q: Can the agent push updates without breaking my Amplience JSON schemas?**
Yes. Before invoking the update tool, the agent utilizes context to retrieve the item's precise configuration. It parses the associated Schema ID requirements and injects the updated stringified payload adhering identically to Amplience's validation rules.

**Q: Will the integration protect my items against concurrent manipulation issues?**
Yes. Our Amplience server requires the agent to explicitly pass the exact `version` lock integer on every DELETE or UPDATE request. If a human colleague alters your CMS page while the agent is typing, the AI request is robustly rejected avoiding fatal overwrites.

**Q: Can I publish a finalized post straight to the Edge Delivery API from here?**
Absolutely. Once the content looks solid offline, just declare 'Publish this content item now.' The agent resolves the `publish_content_item` tool pointing to your Edge API and the post lives dynamically on your core frontend instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amplience](https://vinkius.com/mcp/amplience)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Amplience** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `amplience` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Amplience** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "amplience": {
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
