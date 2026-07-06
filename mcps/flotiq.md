# Flotiq MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flotiq)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage headless content via Flotiq — create and search content objects, handle media assets, audit schemas, and track tenant limits directly from any AI agent.

## Description
Connect your **Flotiq** account to any AI agent and take full control of your API-first headless CMS and structured content delivery through natural conversation.

### What you can do

- **Content Object Orchestration** — Identify bounded routing spaces inside the headless Flotiq CMS and extract explicitly attached REST arrays targeting specific content types natively
- **Live Record Management** — Provision highly-available JSON payloads to write or update Flotiq models, or irreversibly vaporize specific nodes to clear live database bytes
- **Schema Auditing** — Retrieve the exact structural matching for delivery models and enumerate explicitly attached structured rules exporting active type vectors
- **Global Semantic Search** — Execute immediate queries across all content by tapping raw status configurations validating words bounding Elastic/Graph limits flawlessly
- **Media Asset Discovery** — Perform structural extraction of properties driving active media limits by hitting physical CDN uploads mapped in your tenant environment
- **Relational Data Hydration** — Analyze specific ID configurations mapping to internal dependencies and parsing relations securely through hydrated object retrieval
- **Tenant Oversight** — Identify precise active arrays spanning your rented identity limits, analyzing quotas and base endpoints available synchronously

### How it works

1. Subscribe to this server
2. Enter your Flotiq API Key (found in your Flotiq Dashboard > API Keys)
3. Start managing your structured content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Editors & Managers** — create and update content objects and manage media assets without the Flotiq editor UI
- **Full-stack Developers** — test and debug API-first content models and verify schema mappings directly from the IDE
- **Product Teams** — monitor tenant limits and verify content type definitions using natural language conversation
- **Digital Marketers** — search across global content and manage media libraries through natural conversation


## Available Tools (10)
- **get_content_type_schema**: Retrieve the exact structural matching verifying Delivery Model blocks
- **get_tenant_limits**: Identify precise active arrays spanning rented Identity limits
- **list_content_objects**: Identify bounded routing spaces inside the Headless Flotiq CMS
- **list_media_assets**: Perform structural extraction of properties driving active Media limits
- **list_all_content_types**: Enumerate explicitly attached structured rules exporting active Type vectors
- **search_global_content**: Inspect deep internal arrays mitigating specific Picture constraints
- **patch_cms_object**: Mutate global Web CRM boundaries substituting Attributes safely
- **create_cms_object**: Provision a highly-available JSON Payload writing models natively
- **wipe_cms_object**: Irreversibly vaporize explicit App nodes dropping live Database bytes
- **get_content_details**: Retrieve explicit Cloud logging tracing explicit Payload IDs limitlessly


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flotiq** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all items of content type 'blogpost'"

**🤖 AI Agent:**
> Retrieving blogposts... I found 12 objects including 'Intro to MCP' (ID: 1) and 'AI Workflows' (ID: 2). I can retrieve the full hydrated details for any of these records.

---

**👤 You:**
> "Show me the JSON schema for content type 'product'"

**🤖 AI Agent:**
> Retrieving schema for 'product'... This type includes fields: 'name' (string), 'price' (number), 'description' (richtext), and 'image' (datasource). I can use this structure to help you create new product objects.

---

**👤 You:**
> "Search global content for 'feature launch'"

**🤖 AI Agent:**
> Searching global content... I found 3 matches including a 'blogpost' titled 'March Feature Update' and a 'newsletter' entry. Would you like the IDs or snippets for these matches?


## ❓ FAQ

**Q: Can my agent list all available content types in Flotiq?**
Yes. Use the 'list_all_content_types' tool. The agent executes bulk iterations to track explicitly registered types and returns the mapping configured in your Flotiq architecture.

**Q: How do I create a new content object using a JSON payload via chat?**
Use the 'create_cms_object' tool. Provide the 'content_type' and your 'payload_json'. The agent will command the backend to persist the new node utilizing your schema constraints flawlessly.

**Q: Can I search across all my global content through the agent?**
Absolutely. Use the 'search_global_content' tool. Your agent will execute immediate queries across all content by tapping raw status configurations and searching Elastic/Graph limits natively.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flotiq](https://vinkius.com/mcp/flotiq)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flotiq** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flotiq` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flotiq** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flotiq": {
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
