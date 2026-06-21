# DOJ Civil Rights Data MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/doj-civil-rights-data)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/doj-civil-rights-data-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/doj-civil-rights-data-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access Department of Justice civil rights data, including blog entries and press releases, directly from your AI agent.

## Description
Connect your AI agent to the **U.S. Department of Justice (DOJ)** open data portal to query and retrieve critical information regarding civil rights, legal updates, and official announcements.

### What you can do

- **Blog Insights** — List and filter DOJ blog entries by title or date to stay informed on civil rights topics.
- **Press Releases** — Access the latest official press releases and filter them for specific legal components or keywords.
- **Detailed Retrieval** — Fetch the full body, metadata, and associated topics for any specific entry using its unique UUID.
- **Data Sorting** — Organize results by creation date, change date, or relevance to find exactly what you need.

### How it works

1. Subscribe to this server
2. Enter your DOJ API Key (if required) or use the public endpoint configuration
3. Start querying legal data from Claude, Cursor, or any MCP client

### Who is this for?

- **Legal Researchers** — quickly find specific case updates and civil rights announcements without manual searching.
- **Journalists** — monitor official DOJ communications and press releases in real-time.
- **Policy Analysts** — aggregate and analyze trends in DOJ blog topics and public statements.


## Available Tools
- **list_blog_entries**: Use parameters to filter by Civil Rights data (e.g., title="Civil Rights").

List DOJ blog entries
- **get_blog_entry**: Get a specific DOJ blog entry by UUID
- **get_press_release**: Get a specific DOJ press release by UUID
- **list_press_releases**: Use parameters to filter by Civil Rights data.

List DOJ press releases


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DOJ Civil Rights Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the 10 most recent DOJ blog entries about 'Civil Rights'."

**🤖 AI Agent:**
> I've found the latest blog entries. Recent titles include 'Protecting Voting Rights' and 'Advancing Disability Justice'. Would you like the full content of any of these?

---

**👤 You:**
> "Find press releases from the DOJ and sort them by date in descending order."

**🤖 AI Agent:**
> I've retrieved the latest press releases sorted by date. The most recent is 'Justice Department Announces Settlement...' followed by 'Attorney General Statement on...'.

---

**👤 You:**
> "Get the full content for the DOJ blog entry with UUID '550e8400-e29b-41d4-a716-446655440000'."

**🤖 AI Agent:**
> Fetching details for blog entry 550e8400... The entry is titled 'Civil Rights Division Update' and discusses recent enforcement actions. The full body text is now available.


## Installation & Usage

To install and use the **DOJ Civil Rights Data** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/doj-civil-rights-data](https://vinkius.com/mcp/doj-civil-rights-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
