# Tettra MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tettra)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tettra-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tettra-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Tettra** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tettra](https://vinkius.com/mcp/tettra)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
