# Tettra MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tettra)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Search, read, and create internal wiki pages on your Tettra knowledge base directly from your AI agent.

## Description
Connect your **Tettra** internal knowledge base to any AI agent and bring your company's documentation directly into your developer workflow. No more switching tabs to look up API specs or onboarding guides.

### What you can do

- **Deep Search** — Perform full-text searches across all your company's Tettra pages to instantly find answers and organizational knowledge
- **Knowledge Retrieval** — Read the complete markdown/HTML content of any page, technical guide, or team policy natively inside your chat
- **Content Creation** — Command your agent to draft and publish new wiki pages, or suggest documentation updates on the fly
- **Category Navigation** — Browse through your team's top-level categories, root folders, and subcategories visually
- **Q&A Management** — Post new questions to your team's internal Q&A board or list unanswered questions right from your IDE

### How it works

1. Subscribe to this server
2. Enter your Tettra Team ID and API Key (Professional/Scaling plans required)
3. Query your company's brain trust seamlessly from Claude, Cursor, or any MCP-compatible platform

### Who is this for?

- **Software Engineers** — look up internal architecture decisions or environment setup steps without leaving Cursor
- **Operations Leads** — rapidly generate and publish standard operating procedures (SOPs) via AI dictation
- **Product Teams** — maintain robust documentation by verifying outdated pages and suggesting new articles via chat


## Available Tools (12)
- **create_wiki_page**: Provide title, content, and category ID.

Creates a new wiki page in a specific category
- **create_qa_question**: Posts a new question in the Tettra Q&A system
- **get_category_details**: Retrieves details for a specific Tettra category
- **get_page_content**: Returns title and Markdown/HTML body.

Retrieves the full content and metadata of a specific Tettra page
- **list_categories**: Lists all top-level categories in the Tettra wiki
- **list_pages_in_category**: Lists all wiki pages within a specific category
- **list_qa_questions**: Lists all questions posted in the Tettra Q&A system
- **list_subcategories**: Lists all subcategories under a specific parent category
- **search_pages**: Returns up to 5 matching pages.

Full-text search across all Tettra wiki pages
- **suggest_new_page**: Suggests a new wiki page to the team
- **update_wiki_page**: Provide the page ID and the new fields.

Updates the title or content of an existing Tettra page
- **verify_wiki_page**: Marks a Tettra page as verified and up-to-date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tettra** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search the wiki for 'Database Migration Checklist'."

**🤖 AI Agent:**
> I found 1 relevant page in the wiki:
- **Database Migration Checklist** (ID: 1042) in the 'Engineering' category.
Would you like me to fetch the full markdown content of this guide?

---

**👤 You:**
> "Create a new wiki page in the 'Support' category explaining how to handle refund requests."

**🤖 AI Agent:**
> Successfully published page **Refund Handling Procedure** (ID: 4055) to the Support category (ID: 12)!
The content has been formatted with step-by-step markdown. Your team can now search for it natively on Tettra.

---

**👤 You:**
> "Mark page ID 883 as verified and up to date."

**🤖 AI Agent:**
> The page 'Deployment Keys Matrix' (ID 883) has been officially verified! ✅
The system will log that it was verified today, maintaining trust in your knowledge base.


## ❓ FAQ

**Q: Why do I get an error when providing my token?**
Tettra's API keys are exclusively available to workspaces on their **Scaling** or **Professional** subscription tiers. If your team operates on a free or basic plan, the API credentials menu will not be accessible and requests will be blocked.

**Q: Can the AI rewrite existing company wiki articles?**
Yes. Using the `update_wiki_page` function, the AI can overwrite existing body content and titles. It adopts your user profile's access permissions, meaning it can only update pages you personally have edit rights for in the Tettra UI.

**Q: Where do I track down my Tettra Team ID?**
Your Team ID is the slug prefix used in your Tettra domain. For example, if you access your wiki primarily through `https://app.tettra.co/teams/acme-corp`, your Team ID is exactly `acme-corp`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tettra](https://vinkius.com/mcp/tettra)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tettra** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tettra` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tettra** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tettra": {
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
