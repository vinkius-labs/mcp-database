# Zesty.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zestyio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage content models, items, and instances via the Zesty.io API.

## Description
Connect your **Zesty.io** account to any AI agent to streamline your headless CMS operations. This MCP server enables your agent to interact with instances, content models, and data entries (items) directly from natural language.

### What you can do

- **Instance Oversight** — List all Zesty.io instances associated with your account and retrieve their metadata
- **Schema Management** — List content models to understand your data structures and identify Model ZUIDs
- **Content Operations** — List, retrieve, create, and update content items within specific models
- **Technical Auditing** — Access instance settings and technical metadata for any of your properties
- **Workflow Automation** — Delete content items and maintain your CMS hierarchy via natural language commands

### How it works

1. Subscribe to this server
2. Enter your Zesty API Token and Instance ZUID (starting with 8-)
3. Start managing your content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Managers** — Update website content and manage entries without logging into the Zesty interface
- **Developers** — Quickly query content models and test API data structures from your IDE
- **Growth Engineers** — Automate the creation of landing page items and marketing content entries


## Available Tools (8)
- **create_content_item**: Requires a JSON object with field values.

Create a new content item
- **delete_content_item**: Delete a content item
- **get_content_item**: Get details for a specific content item
- **list_zesty_instances**: List all Zesty.io instances associated with the account
- **list_content_items**: List content items for a specific model
- **list_content_models**: Use this to identify Model ZUIDs.

List all content models for the current instance
- **get_instance_settings**: Get configuration settings for the instance
- **update_content_item**: Update an existing content item


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zesty.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all Zesty instances I have access to."

**🤖 AI Agent:**
> I've retrieved your instances. You have access to 3 properties: 'Corporate Blog' (ZUID: 8-abc-123), 'Product Showcase' (ZUID: 8-xyz-456), and 'Marketing Landing Pages' (ZUID: 8-def-789).

---

**👤 You:**
> "Show me the content items for the 'Press Releases' model (ZUID: '6-ghi-987')."

**🤖 AI Agent:**
> I found 5 items in the 'Press Releases' model. Recent titles include 'Q3 Earnings Report' and 'New Partnership Announcement'. Would you like to see the details for any of them?

---

**👤 You:**
> "Update the title of content item '7-jkl-654' in model '6-ghi-987' to '2024 Product Roadmap'."

**🤖 AI Agent:**
> Successfully updated content item '7-jkl-654'. The new title is now '2024 Product Roadmap' in your Zesty instance.


## ❓ FAQ

**Q: How do I find my Instance ZUID?**
You can list all your accessible instances using the `list_zesty_instances` tool, or find it in your Zesty.io URL (it starts with `8-`).

**Q: Can I see all content items for a particular model?**
Yes, use the `list_content_items` tool with the unique ZUID of the model (starts with `6-`) to retrieve all associated entries.

**Q: Is it possible to update content via the agent?**
Absolutely. Use the `update_content_item` tool by providing the Model ZUID, the Item ZUID, and a JSON object containing the fields you wish to modify.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zestyio](https://vinkius.com/mcp/zestyio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zesty.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zestyio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zesty.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zestyio": {
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
