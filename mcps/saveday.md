# SaveDay MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/saveday)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Capture, organize, and summarize content from URLs, text, and images directly into your SaveDay knowledge base.

## Description
Connect your **SaveDay** account to any AI agent to seamlessly capture and retrieve information. SaveDay acts as your second brain, allowing you to store web content, notes, and images, and then query them using natural language.

### What you can do

- **Content Capture** — Instantly save URLs, text snippets, or images with custom titles and tags using the `capture_content` tool.
- **Smart Search** — Query your saved items using natural language with `search_items` to find exactly what you need without manual sorting.
- **AI Summarization** — Use `get_summary` to generate concise summaries of your saved content to grasp key points quickly.
- **Tag Management** — List and organize your knowledge base using the `list_tags` tool for better categorization.

### How it works

1. Subscribe to this server
2. Enter your SaveDay API Key
3. Start capturing and searching your knowledge base from Claude, Cursor, or any MCP-compatible client.


## Available Tools
- **capture_content**: Type must be url, text, or image.

Capture a URL, text, or image to SaveDay
- **search_items**: Search through saved items
- **get_summary**: Retrieve an AI-generated summary for a specific saved item
- **list_tags**: Retrieve a list of all tags used in the SaveDay account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SaveDay** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Save this URL to my SaveDay with the tag 'research': https://example.com/ai-mcp"

**🤖 AI Agent:**
> I've successfully captured the content from the URL. It has been saved to your SaveDay account with the tag 'research'.

---

**👤 You:**
> "Search my SaveDay for any notes about 'smart home automation'."

**🤖 AI Agent:**
> I found 3 items related to 'smart home automation'. Would you like me to summarize the most recent one or list them all?

---

**👤 You:**
> "Show me all the tags I have used in SaveDay."

**🤖 AI Agent:**
> Here are your current tags: 'research', 'work', 'recipes', 'travel', and 'ai-tools'.


## ❓ FAQ

**Q: Can I search my saved items using natural language?**
Yes! Use the `search_items` tool with your query. The AI will search through your saved content to find the most relevant items based on your keywords or natural language description.

**Q: How do I get a quick overview of a long article I saved?**
You can use the `get_summary` tool by providing the unique ID of the saved item. SaveDay will return an AI-generated summary highlighting the most important information.

**Q: What types of content can I save to SaveDay?**
The `capture_content` tool supports three types: 'url' for websites, 'text' for snippets or notes, and 'image' for base64 encoded images. You can also optionally provide a title and tags.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/saveday](https://vinkius.com/mcp/saveday)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SaveDay** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `saveday` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SaveDay** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "saveday": {
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
