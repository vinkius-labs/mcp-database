# Browser Bookmarks Parser MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/browser-bookmarks-parser)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Turn messy Chrome, Safari, and Firefox bookmark HTML exports into clean, structured JSON data. Instantly allow your AI to organize your digital life and remove duplicate links.

## Description
You have thousands of bookmarks saved over the years. You export them from your browser, hoping Claude can help you organize them, find dead links, or group them by topic. But the export is a massive, unreadable 'Netscape Bookmark' HTML file. If the AI tries to read it, it hallucinates folder structures and runs out of context tokens.

This MCP uses a fast, deterministic parser to convert that legacy HTML format into a beautifully structured JSON hierarchy. It completely strips away the DOM noise and returns exactly what your agent needs: Folders, Titles, and URLs.

### The Superpowers

- **Universal Support:** Parses native exports from Google Chrome, Safari, Firefox, Edge, and Arc.
- **Hierarchy Preserved:** Deeply nested folders are correctly mapped into the JSON structure.
- **Zero Hallucination:** No more guessing where a folder ends and a link begins.
- **Digital Decluttering:** Turns Claude into your personal librarian. Say: 'Read my bookmarks and remove all duplicate URLs'.


## Available Tools (1)
- **parse_browser_bookmarks**: Provide the absolute file path to the .html export file.

Parse a messy Netscape Bookmark HTML file (exported from Chrome, Safari, Firefox) into clean, structured JSON


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Browser Bookmarks Parser** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Read my exported bookmarks.html and list all the duplicate URLs."

**🤖 AI Agent:**
> I analyzed your bookmarks and found 14 duplicate URLs across 3 different folders. Would you like me to generate a script to remove them?

---

**👤 You:**
> "Look at my bookmarks file and group all the links that look like AI tools into a new suggested folder structure."

**🤖 AI Agent:**
> I've analyzed your 450 bookmarks. Here is a suggested folder structure for the 42 AI-related tools you saved:
- /AI Image Generators/
- /LLM APIs/

---

**👤 You:**
> "Extract only the bookmarks from the 'Read Later' folder and format them as a Markdown list."

**🤖 AI Agent:**
> Here is your 'Read Later' list:
- [TechCrunch Article](https://techcrunch.com/...)
- [React Documentation](https://react.dev/...)


## ❓ FAQ

**Q: Does it keep my nested folder structure?**
Yes! The parser strictly maintains the exact folder hierarchy (e.g., 'Work -> Q3 Reports -> Sales.pdf') so the AI understands exactly how your bookmarks are categorized.

**Q: Is my browsing data sent to the cloud?**
No. The HTML parsing happens 100% locally on your machine. The engine only feeds the clean JSON representation back to your AI chat context.

**Q: Can it identify broken links or 404 pages?**
While the parser itself just extracts the URLs local, you can subsequently ask Claude to use a network tool to test if the extracted links are still active.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/browser-bookmarks-parser](https://vinkius.com/mcp/browser-bookmarks-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Browser Bookmarks Parser** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `browser-bookmarks-parser` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Browser Bookmarks Parser** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "browser-bookmarks-parser": {
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
