# DOJ Civil Rights Data MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/doj-civil-rights-data)
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


## ❓ FAQ

**Q: Can I filter blog entries by a specific topic like 'Civil Rights'?**
Yes. Use the `list_blog_entries` tool and set the `title` parameter to 'Civil Rights'. This will return entries matching that specific keyword.

**Q: How do I get the full text of a press release?**
Once you have the UUID from a list, use the `get_press_release` tool with that `uuid`. It will return the full body, URL, and metadata.

**Q: Can I control how many results are returned per query?**
Yes, use the `pagesize` parameter (default 20, max 50) and the `page` parameter to navigate through the results.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/doj-civil-rights-data](https://vinkius.com/mcp/doj-civil-rights-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DOJ Civil Rights Data** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `doj-civil-rights-data` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DOJ Civil Rights Data** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "doj-civil-rights-data": {
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
