# Magnolia (Enterprise Headless CMS) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/magnolia-enterprise-headless-cms)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage enterprise content via Magnolia CMS — query JCR nodes, audit template schemas, and orchestrate headless delivery.

## Description
Connect your **Magnolia CMS** instance to any AI agent and take full control of your enterprise-grade headless content and JCR repository management through natural conversation.

### What you can do

- **Node Orchestration** — List, retrieve, and create hierarchical JCR nodes directly from your agent, allowing for precise structural content management
- **JCR Discovery** — Execute complex property-based queries using native JCR logic to identify specific content fragments and textual mappings securely
- **Template Schema Audit** — Extract detailed component and page template definitions to understand which fields and properties a component expects natively
- **Delivery Layer Management** — Navigate through explicitly configured delivery endpoints (e.g., pages, tours) to verify JSON mappings and content boundaries
- **Workspace Visibility** — Discover and list active JCR workspaces (website, dam, configuration) to understand how your project data is distributed
- **Operational Commands** — Trigger automated workspace commands including activation and publishing workflows to move content through its lifecycle
- **Cloning & Relocation** — Copy or move content nodes across your repository while maintaining structural matching and delivery logic integrity

### How it works

1. Subscribe to this server
2. Enter your Magnolia Host, Port, and Basic Auth (Base64)
3. Start managing your enterprise repository from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Headless Developers** — test delivery API results and verify JCR node properties through natural conversation without manual REST tools
- **Content Architects** — audit component schemas and manage hierarchical content trees across multiple site environments efficiently
- **Digital Ops Teams** — monitor workspace health and execute publishing commands across your entire Magnolia instance


## Available Tools (10)
- **mg.copy_delivery_node**: Retrieve the exact structural matching verifying Delivery cloning logic
- **mg.create_cms_node**: Provision a highly-available JSON Payload writing models natively
- **mg.wipe_cms_node**: Irreversibly vaporize explicit App nodes dropping live Database bytes
- **mg.execute_workspace_command**: Dispatch an automated validation check routing explicit Platform logic
- **mg.get_delivery_children**: Perform structural extraction of properties driving active Branch nesting
- **mg.get_delivery_node**: rest/delivery/ENDPOINT/PATH` returning pure JSON mappings from the JCR tree securely.

Identify bounded routing spaces inside the Headless Magnolia Delivery layers
- **mg.get_template_schema**: Enumerate explicitly attached structured rules exporting active fields
- **mg.list_jcr_workspaces**: Identify precise active arrays spanning rented Context domains
- **mg.query_delivery_nodes**: Retrieve explicit Cloud logging tracing explicit Payload criteria
- **mg.patch_cms_node**: Mutate global Web CRM boundaries substituting Draft Document schemas


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Magnolia (Enterprise Headless CMS)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the node details for path 'tours/bali' from the 'tours_v1' delivery endpoint"

**🤖 AI Agent:**
> Retrieving node '/tours/bali'… I've fetched the JSON mapping. It contains properties like tourName: 'Exotic Bali', price: 1200, and duration: '10 days'. Would you like to see the child nodes or the associated template definition?

---

**👤 You:**
> "List all active JCR workspaces in our Magnolia instance"

**🤖 AI Agent:**
> I've identified the following workspaces: 'website' (Site content), 'dam' (Assets), 'configuration' (System settings), 'imaging' (Image processing), and 'categorization' (Tags). Which one would you like to explore?

---

**👤 You:**
> "Show me the schema definition for template 'mgnl-news-article'"

**🤖 AI Agent:**
> Retrieving schema for 'mgnl-news-article'… This template expects 4 main fields: 'title' (Required, Text), 'body' (RichText), 'image' (Link to DAM), and 'author' (Text). I can help you create a new node implementing this structure.


## ❓ FAQ

**Q: Can I navigate the JCR tree structure through my agent?**
Yes. Use the `mg.get_delivery_children` tool by providing an endpoint and parent path. Your agent will retrieve exclusively the hierarchical descendants, allowing you to understand the branch nesting and property distribution accurately.

**Q: How do I audit the required fields for a specific Magnolia component?**
The `mg.get_template_schema` tool parses the YAML definitions of your components. Your agent will list exactly what fields and scalar parameters the template respects, making it easy to verify your content model without opening the code.

**Q: Can my agent trigger a content publication command?**
Absolutely. Use the `mg.execute_workspace_command` tool and specify 'activate' or 'publish' as the command name. Your agent will dispatch the JSON payload to Magnolia's command system to transition your content across lifecycle states.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/magnolia-enterprise-headless-cms](https://vinkius.com/mcp/magnolia-enterprise-headless-cms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Magnolia (Enterprise Headless CMS)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `magnolia-enterprise-headless-cms` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Magnolia (Enterprise Headless CMS)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "magnolia-enterprise-headless-cms": {
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
