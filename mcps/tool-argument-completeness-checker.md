# Tool Argument Completeness Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tool-argument-completeness-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Audits LLM tool calls to detect missing parameters and value hallucinations.

## Description
This MCP server provides a suite of validation utilities designed to ensure Large Language Models (LLMs) adhere to strict tool schemas. By analyzing raw text, it identifies missing required arguments and detects 'hallucinations' where provided values do not match allowed enumerations. Use `tool_validate_extraction` to compute completeness scores, `tool_get_argument_coverage` for high-level gap analysis, and `tool_extract_raw_matches` for low-level pattern scanning.


## Available Tools (3)
- **tool_extract_raw_matches**: Low-level scan for argument-value pairs
- **tool_get_argument_coverage**: Provides a high-level summary of tool adherence
- **tool_validate_extraction**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tool Argument Completeness Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate this tool call: 'call tool_validate_extraction with actionText="name: John, age: 30" and requiredArguments=["name", "age"]'"

**🤖 AI Agent:**
> {"completenessScore": 100, "missingArguments": [], "hallucinatedArguments": [], "extractedArguments": {"name": "John", "age": "30"}}

---

**👤 You:**
> "Check the coverage for this result: '{"completenessScore": 50, "missingArguments": ["location"], "hallucinatedArguments": [], "extractedArguments": {"name": "Alice"}}'"

**🤖 AI Agent:**
> {"isComplete": false, "gapAnalysis": "Critical: Missing required parameters"}

---

**👤 You:**
> "Extract matches from 'user_id: 123, status: active' using keywords ['user_id', 'status']"

**🤖 AI Agent:**
> {"matches": [{"foundKey": "user_id", "extractedValue": "123"}, {"foundKey": "status", "extractedValue": "active"}]}


## ❓ FAQ

**Q: How does the tool detect hallucinations?**
It compares the extracted argument values against a provided list of valid enums using `tool_validate_extraction`. If a value is found that isn't in the list, it is flagged as a hallucination.

**Q: What is the difference between a missing argument and a hallucination?**
A missing argument is a required field that was not mentioned in the text at all. A hallucination is a field that was mentioned, but with an invalid value that does not match the allowed set.

**Q: Can I use this to scan raw text for any potential values?**
Yes, you can use `tool_extract_raw_matches` to perform a low-level scan of text using specific keywords as anchors to find potential argument-value pairs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tool-argument-completeness-checker](https://vinkius.com/mcp/tool-argument-completeness-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tool Argument Completeness Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tool-argument-completeness-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tool Argument Completeness Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tool-argument-completeness-checker": {
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
