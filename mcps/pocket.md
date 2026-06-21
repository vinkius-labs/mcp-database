# Pocket MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pocket)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pocket-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pocket-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Save articles, videos, and web pages to read later with a personal content library that syncs across all your devices.

## Description
Connect your **Pocket** account to any AI agent and take full control of your digital reading list and knowledge orchestration through natural conversation. Pocket is the premier platform for saving and organizing web content, and this integration allows you to save articles, manage multi-item tags, and archive completed reads directly from your chat interface.

### What you can do

- **Reading List Orchestration** — Save articles, videos, and web pages programmatically with custom titles and tags to ensure your research is always synchronized.
- **Content Organization Intelligence** — Retrieve and filter your saved items by state (unread, archive), content type, or specific tags directly from the AI interface to maintain a high-fidelity library.
- **Metadata & Tag Control** — Add, remove, or rename tags across multiple items via natural language to drive better categorization efficiency.
- **Library Lifecycle Management** — Archive, favorite, or delete items using simple AI commands to keep your reading workflow streamlined.
- **Operational Monitoring** — Track system responses and manage authorization metadata to ensure your content curation is always optimized.

### How it works

1. Subscribe to this server
2. Enter your Pocket Consumer Key and Access Token from your developer portal
3. Start managing your reading list from Claude, Cursor, or any MCP-compatible client

No more manual tagging or losing track of interesting articles. Your AI acts as a dedicated research assistant or knowledge coordinator.

### Who is this for?

- **Researchers & Students** — quickly save and tag relevant papers and articles without switching apps.
- **Content Curators** — automate the organization of inspiration feeds and track high-quality sources via natural conversation.
- **Avid Readers** — streamline the retrieval of unread items and monitor personal knowledge growth directly within the chat.


## Available Tools
- **save_to_pocket**: Save a URL to Pocket
- **add_tags_to_item**: Add labels to item
- **archive_pocket_item**: Archive an item
- **clear_item_tags**: Remove all labels
- **delete_pocket_item**: Permanently remove item
- **favorite_pocket_item**: Mark as favorite
- **list_saved_items**: List your reading list
- **remove_tags_from_item**: Remove labels from item
- **rename_pocket_tag**: Modify tag name
- **search_pocket_list**: Search by keywords
- **test_pocket_auth**: Check connection
- **unfavorite_pocket_item**: Remove from favorites


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pocket** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my last 10 unread items in Pocket."

**🤖 AI Agent:**
> I've retrieved your list. You have 10 unread items including 'Future of AI' and 'Rust Guide'. Which one would you like to tag or archive?

---

**👤 You:**
> "Show me all articles I saved this week organized by tag and reading time."

**🤖 AI Agent:**
> You saved 23 articles this week. By tag: "Tech" (8 articles, avg 7 min read), "Business" (6 articles, avg 12 min), "Design" (5 articles, avg 5 min), "Untagged" (4 articles). Longest read: "The Future of AI Infrastructure" at 24 minutes. 14 articles are still unread. Top source: Hacker News (6 saves), followed by Medium (5) and individual blogs (4). Total estimated reading time: 3 hours 15 minutes.

---

**👤 You:**
> "Archive all articles tagged with Q1 Research that I have already read."

**🤖 AI Agent:**
> 12 articles archived successfully from the "Q1 Research" tag. Articles moved from your reading list to the archive: 8 from Harvard Business Review, 2 from McKinsey Quarterly, 1 from MIT Technology Review, and 1 from Stanford GSB. Average reading time of archived articles: 14 minutes. 3 articles with the same tag remain in your list as they are still marked unread.


## Installation & Usage

To install and use the **Pocket** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pocket](https://vinkius.com/mcp/pocket)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
