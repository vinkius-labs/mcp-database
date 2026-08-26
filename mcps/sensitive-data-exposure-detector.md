# Sensitive Data Exposure Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sensitive-data-exposure-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Intercepts and redacts sensitive information from file reads and tool outputs.

## Description
This MCP server acts as a security layer that intercepts, analyzes, and redacts sensitive information from file reads and tool outputs before they enter the LLM context. It uses deterministic regex patterns to detect AWS keys, GitHub tokens, private keys, database connection strings, and JWTs. It also identifies high-entropy strings using Shannon entropy calculation. By using `scan_content`, users can clean raw text, while `get_redaction_audit` provides a traceable history of all redactions. The `validate_safety_threshold` tool allows for automated security enforcement based on exposure risk scores.


## Available Tools (3)
- **validate_safety_threshold**: Checks if risk meets a threshold
- **get_redaction_audit**: Retrieves the history of redactions
- **scan_content**: Analyzes a raw string for sensitive information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sensitive Data Exposure Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scan this text for secrets: [REDACTED]"

**🤖 AI Agent:**
> The content contains a sensitive AWS key: [REDACTED_AWS:AKIA...XPLE]

---

**👤 You:**
> "Check if this content is safe to use with a threshold of 0.5"

**🤖 AI Agent:**
> The content is not allowed because the exposure risk score exceeds the threshold.

---

**👤 You:**
> "Show me the recent redaction logs."

**🤖 AI Agent:**
> The recent redaction logs show 2 events: one AWS key redaction and one GitHub token redaction.


## ❓ FAQ

**Q: How does the redaction process work?**
The `scan_content` tool identifies sensitive patterns and replaces them with a placeholder in the format `[REDACTED_TYPE:prefix4...suffix4]`. This allows for debugging without exposing the actual secret.

**Q: Can I audit the redactions that have occurred?**
Yes, you can use the `get_redaction_audit` tool to retrieve a history of all redaction events performed during the current session.

**Q: What is the exposure risk score?**
The exposure risk score is a value from 0.0 to 1.0. You can use `validate_safety_threshold` to check if a detected risk exceeds your specific security requirements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sensitive-data-exposure-detector](https://vinkius.com/ai-agent-connect/sensitive-data-exposure-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sensitive Data Exposure Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sensitive-data-exposure-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sensitive Data Exposure Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sensitive-data-exposure-detector": {
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
