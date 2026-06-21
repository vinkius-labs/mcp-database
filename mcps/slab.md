# Slab MCP Server

Manage your team's knowledge base — query wiki articles, create new documentation, and explore topics directly using AI agents.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/slab)

## Overview
**Category:** knowledge-management
**Tools Count:** 12

## Description
Connect your **Slab** workspace to any AI agent and empower your team to search, read, and write documentation seamlessly. Interact with your organization's entire knowledge base through natural language without ever switching tabs.

### What you can do

- **Deep Search & Retrieval** — Execute full-text searches across all Slab posts to fetch answers, guidelines, and protocols instantly
- **Documentation Authoring** — Create new articles, meeting notes, or project specs in Markdown, and update existing posts on the fly
- **Information Architecture** — Browse all your topics (folders) to understand how the company wiki is structured and fetch categorized articles
- **Activity Feeds** — Pull the most recently updated posts to stay on top of new company policies and documentation changes
- **Team Discovery** — Retrieve organization metadata and list all registered team members

### How it works

1. Subscribe to this server
2. Enter your Slab Access Token
3. Start using Claude, Cursor, or any MCP-compatible client to query your company's collective brain

Stop interrupting engineers to ask where a specific document lives. Your AI agent can read the internal wiki and answer questions directly based on your approved Slab content.

### Who is this for?

- **Software Developers** — pull API documentation or architectural guidelines directly into your IDE while coding
- **Product Managers** — instantly draft and publish feature specifications or release notes to the right Slab topic
- **Onboarding & HR** — ask your assistant to fetch the latest company policies or generate reading lists for new hires


## Available Tools
- **list_posts**: Returns post IDs and titles.

List all wiki posts/articles in the Slab workspace
- **get_post_details**: Retrieve the full content and metadata of a specific Slab post
- **search_posts**: Full-text search across all Slab posts
- **list_topics**: List all topics organizing posts in the Slab workspace
- **get_topic_details**: Retrieve details and list of posts for a specific Slab topic
- **list_users**: List all members of the Slab organization
- **get_organization**: Retrieve the Slab organization profile
- **create_post**: Provide content in Markdown.

Create a new wiki post in Slab
- **update_post**: Update an existing Slab post title or content
- **create_topic**: Create a new topic in Slab to organize posts
- **archive_post**: This action is irreversible via API.

Archive an existing Slab post
- **list_recent_posts**: List the most recently updated posts


## Installation & Usage

To install and use the **Slab** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/slab](https://vinkius.com/mcp/slab)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
