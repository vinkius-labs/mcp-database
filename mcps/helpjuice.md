# Helpjuice MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/helpjuice)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Automate knowledge base management via Helpjuice — manage articles, categories, and analytics directly from any AI agent.

## Description
Connect your **Helpjuice** knowledge base to any AI agent and take full control of your internal and external documentation through natural conversation.

### What you can do

- **Article Management** — List all articles, retrieve full content, and create or update documentation directly from the chat.
- **Search Capabilities** — Perform text-based searches across your entire knowledge base to find answers quickly.
- **Content Organization** — List and manage categories to keep your documentation structured and easy to navigate.
- **Analytics Insights** — Retrieve engagement statistics for specific articles and monitor recent search trends.
- **User & Group Oversight** — Access lists of internal contributors and user groups defined for permissions.
- **Interactive Voting** — Record upvotes and downvotes for articles to track content helpfulness.

### How it works

1. Subscribe to this server
2. Enter your Helpjuice API Key and Subdomain
3. Start managing your knowledge base from Claude, Cursor, or any MCP-compatible client

No more manual navigating through complex CMS folders. Your AI assistant acts as a dedicated Knowledge Manager or Documentation Specialist.

### Who is this for?

- **Knowledge Managers** — instantly retrieve article statuses and identify missing or outdated documentation.
- **Support Teams** — check existing documentation and search for answers during customer interactions.
- **Content Creators** — automate the creation of draft articles and monitor engagement stats.


## Available Tools (12)
- **create_article**: Requires a name/title. Pass body fields as a JSON string in "body_json".

Create a new article in the knowledge base
- **downvote_article**: Record a downvote for an article
- **get_article_details**: Get detailed content and metadata for a specific article
- **get_article_stats**: Get engagement statistics for a specific article
- **get_search_trends**: List recent search terms used by visitors
- **list_articles**: Useful for getting a birds-eye view of your content library.

List all articles in the Helpjuice knowledge base
- **list_categories**: List all categories in the knowledge base
- **list_kb_groups**: List user groups defined for permissions
- **list_kb_users**: List all internal users/authors in Helpjuice
- **search_kb**: Useful for finding existing answers to customer questions.

Search the knowledge base for articles matching a query
- **update_article**: Update an existing article
- **upvote_article**: Record an upvote for an article


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Helpjuice** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find articles related to 'OAuth integration'."

**🤖 AI Agent:**
> Searching knowledge base... I found 3 relevant articles: 'Setting up OAuth 2.0', 'API Authentication Guide', and 'Troubleshooting Connection Issues'. Would you like the full content for the 'Setting up OAuth 2.0' article?

---

**👤 You:**
> "List all categories in my knowledge base."

**🤖 AI Agent:**
> I've retrieved your categories. You have 5 main sections: 'Getting Started', 'User Guides', 'Developer API', 'Release Notes', and 'FAQs'. Should I list the articles inside the 'Developer API' category?

---

**👤 You:**
> "Show me the engagement stats for article ID 1021."

**🤖 AI Agent:**
> Retrieving analytics... Article ID 1021 ('Advanced Filtering') has had 450 views and 32 upvotes this month. It is currently one of your top-performing pieces of documentation. Would you like to see recent search terms that led users here?


## ❓ FAQ

**Q: How do I find my Helpjuice API Key?**
Log in to your Helpjuice account, go to **Settings**, and you will find your **API Key** listed in the account or integration section. Ensure you have the necessary permissions to access API settings.

**Q: What is the Helpjuice 'Subdomain'?**
The subdomain is the unique part of your Helpjuice URL (e.g., if your KB is at `mycompany.helpjuice.com`, your subdomain is `mycompany`).

**Q: Can I search for specific terms across my documentation?**
Yes! Use the `search_kb` tool. It performs a real-time search across article titles and body content, returning the most relevant results from your knowledge base.

**Q: Is the integration secure for managing documentation?**
Absolutely. The integration uses official Helpjuice API keys over HTTPS. Your credentials are encrypted and stored securely within the Vinkius Cloud infrastructure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/helpjuice](https://vinkius.com/mcp/helpjuice)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Helpjuice** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `helpjuice` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Helpjuice** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "helpjuice": {
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
