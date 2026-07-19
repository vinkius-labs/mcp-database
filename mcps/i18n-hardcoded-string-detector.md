# i18n Hardcoded String Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/i18n-hardcoded-string-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

An AST-powered auditing tool that identifies un-internationalized text literals in source code by cross-referencing them against translation dictionary keys.

## Description
The i18n Hardcoded String Detector uses advanced Abstract Syntax Tree (AST) parsing to find user-facing text that hasn't been internationalized. It scans your codebase for strings in JSX/HTML nodes, `aria-label` attributes, and UI labels, then compares them against your translation dictionary. Use `analyze_codebase` to extract candidate strings, `verify_dictionary_syntax` to check your JSON/JS files, and `audit_strings` to generate a report of hardcoded violations and orphaned keys.


## Available Tools (3)
- **analyze_codebase**: Identify all candidate user-facing string literals within a given directory
- **audit_strings**: Compare discovered candidate strings against the translation dictionary
- **verify_dictionary_syntax**: Ensure the translation dictionary is structurally sound


## 💬 Prompt Examples

Here are some examples of how you can interact with the **i18n Hardcoded String Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scan my React project for hardcoded strings."

**🤖 AI Agent:**
> I will use `analyze_codebase` on the specified path to identify all candidate UI strings using AST parsing.

---

**👤 You:**
> "Check if my en.json file is valid."

**🤖 AI Agent:**
> I will run `verify_dictionary_syntax` on the provided path to ensure the JSON structure is correct and readable.

---

**👤 You:**
> "Compare these strings against my translation keys."

**🤖 AI Agent:**
> I will use `audit_strings` with the provided candidate strings, dictionary keys, and values to generate a report of hardcoded text and orphaned keys.


## ❓ FAQ

**Q: How does the tool identify strings without using regex?**
The tool performs deterministic AST traversal to distinguish between actual UI text nodes and technical identifiers like CSS classes or console logs.

**Q: Can I use `audit_strings` with any translation format?**
Yes, as long as you provide the extracted keys and values from your dictionary to the tool.

**Q: What does a 'hardcoded' violation mean?**
A violation is flagged when a string literal found in your UI (via `analyze_codebase`) does not exist as a key or value in your translation dictionary.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/i18n-hardcoded-string-detector](https://vinkius.com/mcp/i18n-hardcoded-string-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **i18n Hardcoded String Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `i18n-hardcoded-string-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **i18n Hardcoded String Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "i18n-hardcoded-string-detector": {
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
