# Inoreader MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/inoreader)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Follow hundreds of news sources and blogs with a powerful RSS reader that filters, organizes, and prioritizes content for you.

## Description
Connect your **Inoreader** account to any AI agent and transform how you monitor news, blogs, and social feeds through natural language control.

### What you can do

- **Feed Management** — List all your subscriptions and quickly add new RSS/Atom feeds by URL.
- **Content Extraction** — Fetch article contents from specific feeds, folders, or system streams with advanced filtering.
- **Organization** — List, create, rename, and delete tags or folders to keep your information architecture clean.
- **Engagement** — Star important articles, mark items as read, or batch-clear entire streams instantly.
- **Unread Monitoring** — Get real-time summaries of unread counts across all your categorized content.

### How it works

1. Subscribe to this server
2. Enter your Inoreader Access Token (found in your developer preferences)
3. Start querying and organizing your knowledge base from Claude, Cursor, or any MCP client

### Who is this for?

- **Researchers & Analysts** — aggregate intelligence from hundreds of sources and filter for specific keywords using AI.
- **Content Creators** — monitor industry trends and save inspiration directly to tagged folders without leaving your workspace.
- **Information Junkies** — keep your 'Unread' counts at zero by letting your AI assistant help you prioritize what truly matters.


## Available Tools
- **delete_tag**: Articles will remain but the organizational label is removed.

Delete a tag or folder
- **edit_tag**: Use "user/-/state/com.google/starred" to star/unstar an item.

Add or remove tags from articles (e.g., Starred)
- **get_unread_counts**: Get the number of unread items per feed/folder
- **get_user_info**: Get Inoreader user information
- **list_stream_contents**: Use "user/-/state/com.google/reading-list" for all items.

Get articles for a specific feed, folder, or tag
- **list_subscriptions**: List all user subscriptions (feeds)
- **list_tags**: List all user tags and folders
- **mark_all_as_read**: Mark all items in a stream as read
- **quick_add_subscription**: Subscribe to a new feed by URL
- **rename_tag**: Rename an existing tag or folder


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Inoreader** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the latest news from my Tech folder?"

**🤖 AI Agent:**
> I've fetched the contents of your 'Tech' folder. Here are the top 3 stories: 'New AI Breakthrough' from TechCrunch, 'React 19 Released' from Dev.to, and 'The Future of Web3' from Wired. Would you like me to summarize any of these?

---

**👤 You:**
> "Find articles about 'SpaceX' that I haven't read yet."

**🤖 AI Agent:**
> Searching your unread reading list... I found 2 articles related to SpaceX: 'Starship Test Flight Update' and 'Falcon 9 Launch Schedule'. Both are marked as unread. Shall I open the description for the Starship flight?

---

**👤 You:**
> "Mark all articles in my 'Social Media' tag as read."

**🤖 AI Agent:**
> Processing batch update... Done! All articles within the 'Social Media' tag have been marked as read. Your unread count for this tag is now zero.


## ❓ FAQ

**Q: Can I use this to find specific articles across all my subscriptions?**
Yes! Use the `list_stream_contents` tool with the system stream ID `user/-/state/com.google/reading-list`. You can then ask the AI to filter or search for specific keywords within the returned articles.

**Q: Is it possible to star articles directly from the conversation?**
Absolutely. Use the `edit_tag` tool and provide the Article ID with the add parameter set to `user/-/state/com.google/starred`. This will instantly save the article to your Starred folder in Inoreader.

**Q: How do I see how many unread articles I have in each folder?**
Run the `get_unread_counts` tool. It returns a structured list of all your streams (feeds, folders, and tags) along with the precise count of unread items for each.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/inoreader](https://vinkius.com/mcp/inoreader)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Inoreader** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `inoreader` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Inoreader** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "inoreader": {
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
