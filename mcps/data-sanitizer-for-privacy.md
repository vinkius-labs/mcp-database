# Data Sanitizer for Privacy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/data-sanitizer-for-privacy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Redacts sensitive PII and PHI from text using deterministic patterns.

## Description
This MCP server provides a specialized privacy enforcement layer for AI agents. It identifies and redacts sensitive information such as emails, phone numbers, SSNs, and credit card details using strict regex patterns. You can use `sanitize_text` to perform token-level or sentence-level redaction, ensuring your LLM inputs and outputs remain compliant with data protection standards. Use `validate_entity_type` to check supported categories or `get_redaction_summary` to view all available patterns.


## Available Tools (3)
- **get_redaction_summary**: Provides an overview of the supported redaction patterns
- **sanitize_text**: You can specify which entity types to look for and whether to redact the entire sentence containing the sensitive data.

Redacts sensitive information from text based on specified entity types
- **validate_entity_type**: g., "EMAIL") to check its validity.

Checks if a specific entity type is supported by the sanitizer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Data Sanitizer for Privacy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Sanitize this text: My email is john.doe@example.com and my phone is 555-0199."

**🤖 AI Agent:**
> My email is [EMAIL_REDACTED] and my phone is [PHONE_REDACTED].

---

**👤 You:**
> "Redact the SSN in this sentence: The user's SSN is 123-45-6789."

**🤖 AI Agent:**
> The user's SSN is [SSN_REDACTED].

---

**👤 You:**
> "Check if 'SSN' is a valid entity type for redaction."

**🤖 AI Agent:**
> Yes, SSN is a supported entity type.


## ❓ FAQ

**Q: How does the redaction work?**
The tool uses deterministic regex patterns to find sensitive data and replaces it with a placeholder like `[EMAIL_REDACTED]`. You can also choose to redact the entire sentence containing the sensitive data.

**Q: What entity types can be redacted?**
You can redact various types including EMAIL, PHONE, SSN, and CREDIT_CARD. Use `get_redaction_summary` to see the full list of supported types.

**Q: Can I redact whole sentences?**
Yes, by setting the `redactEntireSentences` parameter to true in the `sanitize_text` tool, the entire sentence containing the sensitive information will be replaced.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/data-sanitizer-for-privacy](https://vinkius.com/mcp/data-sanitizer-for-privacy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Data Sanitizer for Privacy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `data-sanitizer-for-privacy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Data Sanitizer for Privacy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "data-sanitizer-for-privacy": {
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
