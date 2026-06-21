# Confluence MCP Server

Empower your AI agent to search, read, and create Confluence wiki pages directly from chat.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/confluence)

## Overview
**Category:** industry-titans
**Tools Count:** 12

## Description
Connect your **Atlassian Confluence** workspace to your AI assistant. Easily query your organization's knowledge base, search through technical documentation, and seamlessly generate new formatted pages right from the conversational interface.

### What you can do

- **Search Wiki Spaces** — Quickly retrieve specific software architecture decisions, HR policies, or meeting notes without switching tabs.
- **Read Pages** — Extract the complete text and markdown-structured content of existing wiki pages for quick summaries.
- **Create & Publish** — Draft robust product requirements documents (PRDs) or meeting minutes using the AI, and publish them directly to your designated Confluence spaces.

### How it works

1. Install this MCP server integration.
2. Authorize using your Atlassian API Token and registered email.
3. Chat with your AI to explore your company's knowledge base.

### Who is this for?

- **Software Engineers** — Instantly search technical guidelines and architectures without leaving the development environment.
- **Product Managers** — Quickly publish drafted PRDs and sprint notes during planning sessions.
- **Human Resources** — Look up and reference company policies inside conversational threads to assist employees.


## Available Tools
- **add_label**: Labels help organize and filter wiki content.

Add a label to a Confluence page
- **delete_page**: This action is irreversible.

Delete a Confluence page permanently
- **get_page_history**: Retrieve the version history of a Confluence page
- **list_labels**: List all labels on a Confluence page
- **add_page_comment**: The body should be in storage format (HTML).

Add a new comment to a Confluence page
- **search_confluence**: g. text ~ "project" AND type = "page"). Returns matching pages, blog posts, and comments.

Search for content using Confluence Query Language (CQL)
- **create_page**: Requires the space key, a title, and body content in Confluence storage format (HTML). The page is created at the root of the space.

Create a new page in a Confluence space
- **get_page**: Returns content body, space, version history, and metadata.

Retrieve detailed information about a specific page
- **get_space_details**: Returns metadata, description, homepage, and permissions overview.

Retrieve detailed information about a specific space
- **list_page_comments**: Returns inline and footer comments with author and content.

Retrieve all comments for a specific Confluence page
- **list_pages**: Optionally filter by space key. Supports pagination via start offset and limit.

Retrieve a list of pages from Confluence
- **list_spaces**: Retrieve a list of all spaces in Confluence


## Installation & Usage

To install and use the **Confluence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/confluence](https://vinkius.com/mcp/confluence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
