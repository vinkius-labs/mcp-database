# Tettra MCP Server

Search, read, and create internal wiki pages on your Tettra knowledge base directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/tettra)

## Overview
**Category:** brain-trust
**Tools Count:** 12

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


## Installation & Usage

To install and use the **Tettra** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tettra](https://vinkius.com/mcp/tettra)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
