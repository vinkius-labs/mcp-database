# Data Sanitizer for Privacy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/data-sanitizer-for-privacy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Scrub sensitive PII from LLM contexts using deterministic redaction.

## Description
Protect privacy and ensure compliance by removing sensitive information from LLM inputs and outputs. This MCP server provides tools to detect and redact Personal Identifiable Information (PII) such as emails, phone numbers, and SSNs. Use `sanitize_text` to replace sensitive data with deterministic placeholders, or `audit_text_sensitivity` to analyze text density without modification. It supports both entity-level redaction and full sentence redaction to prevent context leakage.


## Available Tools (3)
- **audit_text_sensitivity**: Analyze text to report presence and density of sensitive information without modifying it
- **get_supported_entities**: Returns the list of supported sensitive entity types
- **sanitize_text**: Scrub sensitive information from text based on entity types and intensity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Data Sanitizer for Privacy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you sanitize this text: 'My email is john.doe@example.com and my phone is 555-0199'?"

**🤖 AI Agent:**
> My email is [EMAIL_REDACTED] and my phone is [PHONE_REDACTED]

---

**👤 You:**
> "Check if there is any sensitive data in: 'The user's SSN is 000-00-0000.'"

**🤖 AI Agent:**
> The text contains one sensitive entity of type SSN.

---

**👤 You:**
> "Sanitize this sentence using full sentence redaction: 'Contact me at 555-1234 immediately.'"

**🤖 AI Agent:**
> [REDACTED]


## ❓ FAQ

**Q: What kind of sensitive data can be sanitized?**
The tool can detect and redact various entity types including EMAIL, PHONE, SSN, and CREDIT_CARD. You can check all available types using the `get_supported_entities` tool.

**Q: What is the difference between entity and sentence redaction?**
Entity redaction replaces only the specific sensitive string. Sentence redaction replaces the entire sentence containing the sensitive data to prevent leakage through surrounding context.

**Q: How can I check if a text contains sensitive information without changing it?**
You can use the `audit_text_sensitivity` tool to get a report on the presence and density of sensitive entities without modifying the original text.


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
