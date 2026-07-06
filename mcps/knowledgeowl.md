# KnowledgeOwl MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/knowledgeowl)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage your knowledge base — list articles, search help content, and audit categories.

## Description
Connect your AI agent to **KnowledgeOwl** to streamline the management and retrieval of your support documentation.

### What you can do

- **Instant Content Retrieval** — Quickly fetch the full content of any help article for use in support or research
- **Smart Search** — Search through your entire help center using natural language to find relevant articles
- **Organization Audit** — List and examine your category hierarchy to ensure your documentation is well-structured
- **Project Context** — Access project-wide settings, custom fields, and glossary terms to maintain consistency
- **Template Discovery** — Browse article templates to assist in creating new documentation

### How to setup

1. Subscribe to this server
2. Log in to your KnowledgeOwl account and go to **Your Profile** > **API Key**
3. Copy your API Key and paste it in the configuration
4. Start managing your KB via natural language


## Available Tools (10)
- **get_category_details**: Get details for a specific category
- **search_help_center**: Search for content in the help center
- **list_kb_glossary**: List all glossary terms
- **list_project_settings**: List project-wide settings
- **list_article_templates**: List available article templates
- **list_kb_custom_fields**: List custom fields defined in the project
- **get_kb_project_info**: Get high-level information about the KB project
- **list_kb_articles**: Useful for browsing content structure.

List all articles in the Knowledge Base
- **get_article_content**: Get detailed content for an article
- **list_kb_categories**: List all categories in the project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **KnowledgeOwl** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search my help center for 'SSO setup'"

**🤖 AI Agent:**
> I've found 3 articles about SSO setup: 'Configuring SAML 2.0', 'Okta Integration Guide', and 'Troubleshooting Login Issues'. Which one would you like me to read for you?

---

**👤 You:**
> "List all categories in my Knowledge Base"

**🤖 AI Agent:**
> Your knowledge base has 5 main categories: 'Getting Started', 'User Management', 'API Reference', 'Billing', and 'Integrations'. I can explore any of these for you.

---

**👤 You:**
> "Get the content of the article with ID 'art_123'"

**🤖 AI Agent:**
> Retrieved content for 'User Management Policy'. The article covers user roles, permission levels, and invited user limitations. Would you like a summary of the roles section?


## ❓ FAQ

**Q: Where do I find my KnowledgeOwl API Key?**
Log in to KnowledgeOwl, click on your name in the top right corner, select **Your Profile**, and look for the **API Key** tab.

**Q: Can I read private articles?**
Yes, as long as your API Key has the necessary permissions, the `get_article_content` tool can retrieve any article in your project.

**Q: Does this support Markdown?**
Yes, the presenter renders article titles and high-level status in Markdown for clear reading in your chat client.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/knowledgeowl](https://vinkius.com/mcp/knowledgeowl)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **KnowledgeOwl** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `knowledgeowl` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **KnowledgeOwl** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "knowledgeowl": {
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
