# Browser Bookmarks Parser MCP Server

Turn messy Chrome, Safari, and Firefox bookmark HTML exports into clean, structured JSON data. Instantly allow your AI to organize your digital life and remove duplicate links.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/browser-bookmarks-parser)

## Overview
**Category:** productivity
**Tools Count:** 1

## Description
You have thousands of bookmarks saved over the years. You export them from your browser, hoping Claude can help you organize them, find dead links, or group them by topic. But the export is a massive, unreadable 'Netscape Bookmark' HTML file. If the AI tries to read it, it hallucinates folder structures and runs out of context tokens.

This MCP uses a fast, deterministic parser to convert that legacy HTML format into a beautifully structured JSON hierarchy. It completely strips away the DOM noise and returns exactly what your agent needs: Folders, Titles, and URLs.

### The Superpowers

- **Universal Support:** Parses native exports from Google Chrome, Safari, Firefox, Edge, and Arc.
- **Hierarchy Preserved:** Deeply nested folders are correctly mapped into the JSON structure.
- **Zero Hallucination:** No more guessing where a folder ends and a link begins.
- **Digital Decluttering:** Turns Claude into your personal librarian. Say: 'Read my bookmarks and remove all duplicate URLs'.


## Available Tools
- **parse_browser_bookmarks**: Provide the absolute file path to the .html export file.

Parse a messy Netscape Bookmark HTML file (exported from Chrome, Safari, Firefox) into clean, structured JSON


## Installation & Usage

To install and use the **Browser Bookmarks Parser** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/browser-bookmarks-parser](https://vinkius.com/mcp/browser-bookmarks-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
