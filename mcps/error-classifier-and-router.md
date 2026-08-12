# Error Classifier and Router MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/error-classifier-and-router)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [reliability](../categories/reliability.md)

Classifies LLM and tool errors into a deterministic taxonomy for automated recovery.

## Description
This MCP server provides a standardized way to interpret unpredictable error outputs from Large Language Model (LLM) APIs and local tool executions. It maps specific error signatures to a taxonomy of error categories, which are then paired with a deterministic recovery action. Use `classify_error` to identify the error type, `get_recovery_strategy` to understand the handling logic, or `validate_retry_eligibility` to check if a retry is permitted based on current attempt counts.


## Available Tools (3)
- **classify_error**: Analyzes a specific error signal to categorize it and determine how to recover
- **get_recovery_strategy**: Returns the high-level strategy details for a previously classified error category
- **validate_retry_eligibility**: Determines if a specific attempt is eligible for a retry based on current attempt counts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Error Classifier and Router** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I received a 429 error from the LLM API. What should I do?"

**🤖 AI Agent:**
> The error is categorized as `rate_limit`, and the recommended recovery action is `retry_with_backoff`.

---

**👤 You:**
> "The tool execution failed with a 'TIMEOUT' error. Is it retryable?"

**🤖 AI Agent:**
> The error is categorized as `timeout`, which maps to the `retry_once` recovery action.

---

**👤 You:**
> "I got a 401 error. How should I handle this?"

**🤖 AI Agent:**
> This is an `auth_failure`, and the required recovery action is `reauth`.


## ❓ FAQ

**Q: How does the error classification work?**
The system uses exact string and integer matching on error codes and keyword detection in error messages to map them to categories like `rate_limit` or `auth_failure`.

**Q: Can I use this to automate retries?**
Yes. By using `validate_retry_eligibility`, your agent can determine if it is allowed to retry an operation and how long it should wait.

**Q: What happens if an error is not recognized?**
If the `errorCode` does not match any known pattern in the taxonomy, the `classify_error` tool will throw an error.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/error-classifier-and-router](https://vinkius.com/mcp/error-classifier-and-router)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Error Classifier and Router** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `error-classifier-and-router` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Error Classifier and Router** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "error-classifier-and-router": {
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
