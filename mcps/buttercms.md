# ButterCMS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/buttercms)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Operate Headless publishing via ButterCMS — search your blog posts, extract custom categories, and map collections with any AI agent.

## Description
Connect your **ButterCMS** publishing instance to any AI agent and extract rich text data, marketing pages, and content taxonomy through natural conversation.

### What you can do

- **Blog Posts Intelligence** — Read precise articles via slug, list large arrays, or search full-text indexes to gather knowledge from your blog
- **Taxonomy Extractor** — Dig deep into your configured internal Tags, Authors, and Categories without opening the standard browser console
- **Custom Pages & Collections** — Enumerate explicit structured JSON objects tracking raw page models spanning multiple website layers effortlessly

### How it works

1. Subscribe to this server
2. Enter your ButterCMS API Token from your project's security settings
3. Start fetching high-grade CRM content straight into Claude, Cursor, or any MCP-compatible smart client

No manual database lookups mapping specific Markdown texts. Your AI agent explores your content warehouse for you directly.

### Who is this for?

- **Seo & Marketing Teams** — evaluate existing tag structures, locate authors' articles seamlessly to propose backlinking and improvements
- **Headless Engineers** — debug component structures identifying why specific Custom Page hits aren't rendering the nested JSON output accurately
- **Content Writers** — run rapid scans identifying if an article covering a target keyword already lives stored inside the official knowledge base


## Available Tools
- **search_blog_posts**: Perform structural extraction of properties driving active Keywords
- **search_collection_field**: Identify precise active arrays spanning filtered Collections
- **get_page_layout**: Retrieve the exact structural matching verifying explicit UI routing
- **get_post_details**: Retrieve explicit Cloud logging tracing explicit Post Slugs
- **list_butter_authors**: Dispatch an automated validation check routing CMS Writers
- **list_butter_categories**: Irreversibly analyze explicit CMS structures routing groupings
- **list_global_collections**: Enumerate explicitly attached structured rules exporting Content items
- **list_custom_pages**: Inspect deep internal arrays mitigating specific Page configurations
- **list_blog_posts**: Identify bounded routing spaces inside the Headless ButterCMS Post limit
- **list_butter_tags**: Mutate global Web CRM boundaries mapping Taxonomy hits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ButterCMS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all our globally defined CMS categories and tell me what the main topic is."

**🤖 AI Agent:**
> I've pulled the categories from ButterCMS. You have 'marketing', 'devops', and 'ai'. 'devops' has 45 active related posts, whereas 'marketing' has 30. Would you like me to scan explicit details for one?

---

**👤 You:**
> "Can you fetch the specific details for the article slug 'intro-to-ai-agents'?"

**🤖 AI Agent:**
> Got it. The article 'Intro to AI Agents' is published by Jane Doe natively. It features a ~900 word body with H2 structures exploring LLM bounding frameworks. It currently sits under the 'tech' tag. Everything matches our SEO guidelines.

---

**👤 You:**
> "Perform a deep search natively for all posts containing 'startup scale'."

**🤖 AI Agent:**
> I executed a full-text search against ButterCMS. Two explicit occurrences matched perfectly: 'How to Growth Hack Your Codebase' and 'Year 2 Recap'. Shall I read the context of those hits to adjust our next strategy?


## ❓ FAQ

**Q: Can my AI analyze the full content of an already published article?**
Absolutely. Through the generic get_post_details tool using a targeted URL slug, the agent actively retrieves the article content boundaries directly from ButterCMS, letting you check formatting errors inside the markup natively.

**Q: Does it connect out to our Custom Pages or specifically built Collections?**
Yes. Beyond just basic blog articles, the agent explores specific array bounds pulling the 'list_custom_pages' endpoint isolating pure localized architectures and fields.

**Q: Will it discover writers or tags independently mapping cross-relations?**
Yes! Running standard category lists returns an exact enumeration mapping taxonomy arrays straight into conversational strings. Ask the bot 'Who are our CMS authors?' and watch the results.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/buttercms](https://vinkius.com/mcp/buttercms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ButterCMS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `buttercms` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ButterCMS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "buttercms": {
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
