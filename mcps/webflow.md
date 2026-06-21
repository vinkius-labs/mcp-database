# Webflow MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/webflow)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Equip your AI agent with direct access to Webflow — manage CMS collections, publish sites, and query site analytics without opening the Webflow designer.

## Description
Connect **Webflow** to your AI agent and manage your websites, CMS content, and e-commerce data conversationally.

### What you can do

- **CMS Management** — List, create, update, and delete CMS collection items (blog posts, portfolio entries, product listings) from natural language.
- **Site Publishing** — Trigger site publishes and check publish status across staging and production domains.
- **Collection Schema** — Query collection structures, field types, and validation rules to understand your content model.
- **E-commerce Data** — Retrieve orders, products, and inventory data from Webflow's built-in e-commerce engine.

### How it works

1. Subscribe to the Webflow integration on the marketplace.
2. Generate an API token from your Webflow site (Site Settings → Apps & integrations → API access → Generate API token).
3. Ask your AI agent to manage CMS items, publish your site, or query collections.

### Who is this for?

- **Content Teams** — Publish blog posts and update CMS collections without opening the Webflow designer or asking a developer.
- **Agencies** — Manage multiple client sites, bulk-update CMS content, and trigger publishes from a single conversational interface.
- **E-commerce Operators** — Monitor orders, update product inventory, and manage catalog data directly from your AI agent.


## Available Tools
- **get_user**: Get authorized user info
- **list_collection_items**: List items in a collection
- **create_collection_item**: Create a CMS item
- **list_pages**: List all site pages
- **list_sites**: List all Webflow sites
- **get_site**: Get site details
- **publish_site**: Publish site to production
- **list_collections**: List CMS collections
- **update_collection_item**: Update a CMS item
- **list_domains**: List site domains


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Webflow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all blog posts in my Webflow CMS."

**🤖 AI Agent:**
> I found 24 blog posts in your 'Blog Posts' collection. The 3 most recent are: 'AI in Marketing' (published 2 days ago), 'Product Update Q1' (published last week), and 'Customer Story: Acme Corp' (draft, unpublished).

---

**👤 You:**
> "Publish my Webflow site to production."

**🤖 AI Agent:**
> Site publish triggered successfully. Your changes are now live on mysite.com. Last publish time: 3 seconds ago. Published domains: mysite.com and mysite.webflow.io.

---

**👤 You:**
> "Create a new blog post titled 'How AI Transforms Marketing'."

**🤖 AI Agent:**
> Blog post created in your 'Blog Posts' collection. Title: 'How AI Transforms Marketing'. Slug: how-ai-transforms-marketing. Status: Draft (unpublished). You can ask me to add body content or publish the site when ready.


## ❓ FAQ

**Q: How do I get my Webflow API token?**
Log in to your Webflow Dashboard. Open the site you want to connect and click the **gear icon** to access Site Settings. In the left sidebar, click **Apps & integrations**. Scroll to the **API access** section at the bottom and click **Generate API token**. Name your token, select the required permission scopes (e.g., CMS read/write, Sites publish), and click **Generate token**. Copy it immediately — Webflow will not show the full token again. Each site can have up to 5 tokens. Tokens expire after 365 days of inactivity.

**Q: Can my AI agent publish a blog post to my Webflow site?**
Yes. Your AI agent can create CMS collection items (like blog posts), set all fields including title, body, slug, thumbnail, and publish date, then trigger a site publish — all in one conversation. Perfect for content teams who want to skip the Webflow designer and go from draft to live in seconds.

**Q: What if I manage multiple client sites as an agency?**
Each Webflow site has its own API token, so you can configure multiple integrations — one per client site. This lets your AI agent switch between projects, bulk-update CMS content across sites, or publish changes to specific client domains without mixing data between accounts.

**Q: Can I track e-commerce orders through my AI agent?**
Yes. If you use Webflow's built-in e-commerce, your AI agent can retrieve orders, order details, fulfillment statuses, and product inventory — giving you a real-time view of sales activity without opening the Webflow dashboard or exporting reports.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/webflow](https://vinkius.com/mcp/webflow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Webflow** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `webflow` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Webflow** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "webflow": {
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
