# GitBook MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gitbook)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gitbook-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gitbook-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage technical documentation via GitBook — list organizations and spaces, handle document pages, search content, and audit collections directly from any AI agent.

## Description
Connect your **GitBook** account to any AI agent and take full control of your technical documentation, knowledge sharing, and docs-as-code workflows through natural conversation.

### What you can do

- **Organization & Space Orchestration** — List all organizations and spaces mapped to your GitBook profile to retrieve identifiers and browse your documentation hierarchy natively
- **Page & Content Discovery** — Extracts the full pages hierarchy from any space and reads entire document pages to retrieve technical information flawlessly
- **Semantic & Keyword Search** — Execute cross-page search operations inside your GitBook namespaces to find matching snippets and relevant content using natural language
- **Collection Management** — List collections that group multiple spaces, identifying how different product documentations are organized across your organizations securely
- **Space Metadata Auditing** — Fetch detailed metadata about specific spaces to verify visibility, access rules, and structural configurations synchronously
- **User Profile Oversight** — Extract authenticated profile metadata including name and email to verify permission limits and account contexts natively
- **Knowledge Base Navigation** — Analyze specific localized variables decoding active documentation routes and extracting structural constraints from your GitBook environment

### How it works

1. Subscribe to this server
2. Enter your GitBook API Token (found in your GitBook Developer Settings)
3. Start managing your technical docs from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Technical Writers & Engineers** — search for existing documentation and verify content structure without opening the GitBook interface
- **Product Managers** — audit documentation spaces and collections to analyze knowledge distribution using natural language
- **Customer Support Teams** — quickly search for technical answers across all product spaces to resolve inquiries in real-time
- **Developers** — test and debug documentation integrations and verify page hierarchies through natural conversation


## Available Tools
- **list_organizations**: List all organizations
- **list_spaces**: List spaces in an organization
- **get_space**: Get space details
- **list_pages**: List pages in a space
- **get_page**: Get page content
- **search_content**: Search content in a space
- **list_collections**: List collections in an organization
- **get_me**: Get authenticated user info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GitBook** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all spaces in organization 'org_123'"

**🤖 AI Agent:**
> Retrieving spaces... I found 3 documentation environments in 'org_123': 'API Reference', 'User Guide', and 'Release Notes'. Which one would you like to explore for pages?

---

**👤 You:**
> "Search my GitBook for 'authentication flow'"

**🤖 AI Agent:**
> Searching content... I found several matches in the 'API Reference' space. The most relevant is a page titled 'Auth Overview' (ID: page_abc). Would you like me to retrieve the full content of that page?

---

**👤 You:**
> "Show me the page hierarchy for space 'User-Guide'"

**🤖 AI Agent:**
> Retrieving hierarchy... The 'User Guide' space has a main 'Getting Started' section, followed by 'Dashboard Basics' and 'Advanced Settings'. Each section has multiple nested pages. Would you like the ID for any specific page?


## Installation & Usage

To install and use the **GitBook** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gitbook](https://vinkius.com/mcp/gitbook)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
