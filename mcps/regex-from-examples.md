# Regex from Examples MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/regex-from-examples)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automation](../categories/automation.md)

Generate ranked regular expression candidates from input and extraction pairs.

## Description
This MCP server uses heuristic pattern analysis to generate the top 3 regex candidates based on provided text pairs. By using `generate_regex_candidates`, you can identify patterns for fixed strings, numbers, dates, and emails. You can also use `evaluate_pattern_coverage` to see exactly which examples match or miss a specific pattern, and `analyze_pattern_complexity` to understand the specificity of your regex.


## Available Tools (3)
- **analyze_pattern_complexity**: Classifies a regex pattern into its structural category
- **evaluate_pattern_coverage**: Provides a detailed breakdown of regex performance
- **generate_regex_candidates**: Analyzes input-extraction pairs to produce regex candidates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Regex from Examples** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a regex for these pairs: 'user@mysite.com' -> 'user@mysite.com', 'admin@test.org' -> 'admin@test.org'."

**🤖 AI Agent:**
> The top candidate is `^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$`.

---

**👤 You:**
> "Analyze the complexity of `\d{3}-\d{3}`."

**🤖 AI Agent:**
> The pattern `\d{3}-\d{3}` is classified as NUMERIC with HIGH specificity.

---

**👤 You:**
> "Check coverage for `\d+` on '123' -> '123', 'abc' -> 'abc'."

**🤖 AI Agent:**
> The regex `\d+` successfully matched '123' but failed to match 'abc'.


## ❓ FAQ

**Q: How do I generate a regex?**
Use the `generate_regex_candidates` tool with your input and extraction pairs.

**Q: Can it handle email addresses?**
Yes, the engine detects structural patterns like email addresses using `generate_regex_candidates`.

**Q: How do I know if a regex is accurate?**
Use `evaluate_pattern_coverage` to check for matches and misses against your dataset.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/regex-from-examples](https://vinkius.com/mcp/regex-from-examples)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Regex from Examples** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `regex-from-examples` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Regex from Examples** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "regex-from-examples": {
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
