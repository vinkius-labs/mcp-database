# Open Graph Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/open-graph-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [social-media](../categories/social-media.md)

Generates standardized Open Graph and Twitter Card HTML meta tags from provided metadata.

## Description
The Open Graph Generator MCP server automates the creation of essential social SEO metadata. By using tools like `generate_html_tags_tool`, you can instantly produce complete blocks of HTML `` tags for Open Graph and Twitter Cards. This ensures that when your content is shared on platforms like Facebook, LinkedIn, or X (formerly Twitter), it renders with rich, professional previews including titles, descriptions, and images. Additionally, use `validate_metadata_tool` to check if your metadata meets best practices for length and engagement, and `get_content_types_tool` to discover all supported content categories like website, article, profile, and book.


## Available Tools (3)
- **get_content_types**: Lists all supported content types
- **generate_html_tags**: Generates Open Graph and Twitter meta tags
- **validate_metadata**: Checks if metadata adheres to social media best practices


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Open Graph Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate HTML tags for a blog post titled 'The Future of AI' with description 'Exploring the next decade of intelligence.' at URL 'https://vinkius.com/blog/ai-future' using the article content type."

**🤖 AI Agent:**
> <meta property="og:title" content="The Future of AI" />
<meta property="og:description" content="Exploring the next decade of intelligence." />
<meta property="og:url" content="https://vinkius.com/blog/ai-future" />
<meta property="og:type" content="article" />
<meta name="twitter:card" content="summary" />
<meta name="twitter:title" content="The Future of AI" />
<meta name="twitter:description" content="Exploring the next decade of intelligence." />

---

**👤 You:**
> "Check if my metadata is good: Title: 'My Awesome Website', Description: 'This is a very long description that might be too much for some platforms to display correctly without truncation.'"

**🤖 AI Agent:**
> {
  "isOptimal": false,
  "warnings": [
    "Description is too long"
  ]
}

---

**👤 You:**
> "What are the available content types I can use?"

**🤖 AI Agent:**
> The supported content types are: website, article, profile, and book.


## ❓ FAQ

**Q: What does this tool generate?**
It generates all necessary HTML `<meta>` tags for Open and Twitter Cards (og:title, og:description, etc.) based on the metadata you provide.

**Q: How can I ensure my metadata is optimized for social sharing?**
You can use the `validate_metadata_tool` to check your title and description. It will return an optimality status and specific warnings if your text is too long or too short for optimal display.

**Q: What content types are supported?**
The server supports several types including website, article, profile, and book. You can always retrieve the most up-to-date list using the `get_content_types_tool`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-graph-generator](https://vinkius.com/mcp/open-graph-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Open Graph Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `open-graph-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Open Graph Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "open-graph-generator": {
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
