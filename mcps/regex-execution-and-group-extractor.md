# Regex Execution and Group Extractor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/regex-execution-and-group-extractor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Executes regular expressions against text to extract matches, groups, and indices.

## Description
This MCP server provides a powerful interface for precise text manipulation and pattern matching. By using tools like `execute_regex` and `extract_substring_indices`, AI agents can perform complex string operations such as identifying capture groups, finding exact character offsets, and detecting specific patterns within large datasets. It is particularly useful for parsing structured logs, extracting metadata from unstructured text, or validating route patterns with `match_route`. The server also includes specialized logic to detect 'islands' of content using the `detect_islands` tool, making it an essential bridge for any agent requiring deterministic regex-based data extraction.


## Available Tools (4)
- **detect_islands**: Detects "islands" in a string—tags that contain server:defer or server:only directives
- **execute_regex**: Executes a regular expression against a target text and returns detailed match information
- **extract_substring_indices**: Extracts all occurrences of a specific substring and returns their indices
- **match_route**: Matches a path against a route pattern and extracts parameters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Regex Execution and Group Extractor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Use `execute_regex` to find all email addresses in this text: 'Contact us at support@vinkius.com or admin@example.org'."

**🤖 AI Agent:**
> [{"match": "support@vinkius.com", "start": 24, "end": 43}, {"match": "admin@example.org", "start": 47, "end": 65}]

---

**👤 You:**
> "Extract the indices of the word 'hello' in 'hello world, hello again'."

**🤖 AI Agent:**
> [{"start": 0, "end": 5}, {"start": 13, "end": 18}]

---

**👤 You:**
> "Check if the path '/api/users/123' matches the pattern '/api/:id'."

**🤖 AI Agent:**
> {"params": {"id": "users/123"}}


## ❓ FAQ

**Q: What can I do with the `execute_regex` tool?**
You can run any valid regular expression against a target string to retrieve an array of matches, including capture groups and their exact start and end character positions.

**Q: How does `extract_substring_indices` work?**
It searches for every occurrence of a specific substring within a larger text and returns the precise character indices (start and end) for each instance found.

**Q: What are 'islands' in the context of `detect_islands`?**
Islands are specific segments of text identified by tags containing `server:defer` or `server:only` directives, which the tool can isolate and report.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/regex-execution-and-group-extractor](https://vinkius.com/mcp/regex-execution-and-group-extractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Regex Execution and Group Extractor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `regex-execution-and-group-extractor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Regex Execution and Group Extractor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "regex-execution-and-group-extractor": {
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
