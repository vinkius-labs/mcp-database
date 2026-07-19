# Annotation Extractor and Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/annotation-extractor-and-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automatically detect, track, and report code annotations like FIXME, HACK, and XXX in your codebase.

## Description
The Annotation Extractor and Tracker MCP server provides a way to manage technical debt by scanning your source files for intentional markers. Using the `scan_file` tool, you can inspect individual files for specific annotations like FIXME or HACK. For larger-scale analysis, use `process_annotations` to compare current file states against previous scans, allowing you to identify resolved tasks and track annotation density across your project. This bridge connects your AI agent directly to your codebase's maintenance needs.


## Available Tools (2)
- **process_annotations**: Processes multiple files to extract and compare annotations
- **scan_file**: Scans a single file for TODO, FIXME, HACK, or XXX annotations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Annotation Extractor and Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scan this file for any pending tasks: /src/index.ts"

**🤖 AI Agent:**
> Found 2 annotations in /src/index.ts: FIXME (line 10) and HACK (line 45).

---

**👤 You:**
> "Check if any markers from my last scan have been resolved."

**🤖 AI Agent:**
> The comparison shows that 3 annotations, including a FIXME on /src/utils.ts, have been resolved.

---

**👤 You:**
> "What is the annotation density in the /src directory?"

**🤖 AI Agent:**
> The density report shows 5 annotations in /src/engine/index.ts and 2 in /src/agents/tool.ts.


## ❓ FAQ

**Q: What types of annotations can this server detect?**
It detects standard markers including `FIXME`, `HACK`, and `XXX` annotations.

**Q: How can I identify if a task has been completed?**
By using the `process_annotations` tool with a reference from a previous scan, you can see which annotations are now resolved.

**Q: Can I analyze a single file or an entire directory?**
You can use `scan_file` for individual files or `process_annotations` to handle batch data for multiple files.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/annotation-extractor-and-tracker](https://vinkius.com/mcp/annotation-extractor-and-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Annotation Extractor and Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `annotation-extractor-and-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Annotation Extractor and Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "annotation-extractor-and-tracker": {
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
