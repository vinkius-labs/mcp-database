# Output Format Contract Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/output-format-contract-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [validation](../categories/validation.md)

Enforces strict data integrity and schema conformity between LLM pipeline stages.

## Description
The Output Format Contract Checker ensures data integrity in LLM-driven pipelines like CrewAI or LangChain. It prevents downstream execution failures by verifying that the output of one stage strictly adheres to a predefined schema. Using the `validate_contract` tool, it performs recursive validation of types, nullability, and enum constraints. It also provides tools like `get_violation_summary` to aggregate errors and `check_coercion_possibility` to identify if simple type casting can resolve mismatches.


## Available Tools (3)
- **check_coercion_possibility**: Checks if a value can be coerced to a target type
- **get_violation_summary**: Aggregates violations into a summary
- **validate_contract**: Validates output data against an expected schema


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Output Format Contract Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate this data: {"id": "123"} against schema {"id": "integer"}"

**🤖 AI Agent:**
> {"is_compliant": false, "violations": [{"path": "id", "type": "type_mismatch"}], "auto_coercible": true}

---

**👤 You:**
> "Check if the value 'true' can be coerced to a boolean."

**🤖 AI Agent:**
> {"can_coerce": true, "suggested_type": "boolean"}

---

**👤 You:**
> "Summarize these violations: [{"type": "missing_field"}, {"type": "type_mismatch"}]"

**🤖 AI Agent:**
> {"total_violations": 2, "missing_count": 1, "type_mismatch_count": 1, "null_violation_count": 0, "enum_violation_count": 0, "extra_field_count": 0}


## ❓ FAQ

**Q: What does this MCP do?**
It validates that JSON data produced by an AI agent matches a specific schema, checking for missing fields, type mismatches, and enum violations using `validate_contract`.

**Q: Can it fix schema errors automatically?**
It identifies if errors are fixable via `check_coercion_possibility`, which checks for simple type conversions like string to integer.

**Q: How do I see a summary of all errors?**
You can use the `get_violation_summary` tool to get a categorized report of all detected contract breaches.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/output-format-contract-checker](https://vinkius.com/ai-agent-connect/output-format-contract-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Output Format Contract Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `output-format-contract-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Output Format Contract Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "output-format-contract-checker": {
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
