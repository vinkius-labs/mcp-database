# Tool Argument Completeness Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tool-argument-completeness-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Extracts and validates tool arguments from LLM action text.

## Description
The Tool Argument Completeness Checker is a specialized MCP server designed to bridge the gap between an LLM's proposed tool call and its actual execution requirements. By analyzing raw action text, it uses regex-based extraction and keyword indexing to identify exact string matches for required arguments. The server computes a missing-parameter percentage, flags required fields that were left null, and detects hallucinated enum values by comparing extracted data against a provided set of valid enums. This is essential for ensuring high reliability in agentic workflows where parameter accuracy is critical.


## Available Tools (1)
- **check_argument_completeness**: Checks if the proposed action text contains all required arguments and detects hallucinations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tool Argument Completeness Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this action is complete: 'Call create_user with name="John" and role="admin"'. Required args: ["name", "role"]. Valid enums: {"role": ["user", "admin"]}."

**🤖 AI Agent:**
> The completeness report shows 100% argument coverage. Both 'name' and 'role' were found, and 'admin' is a valid enum value.

---

**👤 You:**
> "Analyze: 'Update order 123 with status="shipped"'. Required args: ["order_id", "status"]. Valid enums: {"status": ["pending", "shipped"]}."

**🤖 AI Agent:**
> The completeness report shows 100% argument coverage. The 'order_id' was extracted as 123 and 'status' as 'shipped'.

---

**👤 You:**
> "Check: 'Delete item with id="abc"'. Required args: ["id", "reason"]. Valid enums: {}"

**🤖 AI Agent:**
> The completeness report shows 50% argument coverage. The 'id' was found, but the required field 'reason' is missing.


## ❓ FAQ

**Q: How does the tool detect hallucinated values?**
The `check_argument_completeness` tool compares any extracted argument values against a provided JSON object of valid enums. If an extracted value is not present in the allowed set, it is flagged as a hallucination.

**Q: What input format is required for arguments?**
You must provide `requiredArgsJson` as a JSON array of strings and `validEnumsJson` as a JSON object mapping argument names to arrays of allowed values.

**Q: Can it handle complex action text?**
Yes, the tool uses regex and keyword indexing to parse unstructured text, making it capable of extracting values from natural language descriptions of tool calls.


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
