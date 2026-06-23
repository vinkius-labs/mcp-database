# Strict PII Redaction Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/strict-pii-redaction-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Instantly strip sensitive personal data from documents using deterministic, bulletproof regex patterns before AI processing.

## Description
Sending raw legal or financial documents to LLMs risks massive data privacy breaches and compliance violations (GDPR/CCPA). Relying on an LLM to "forget" or manually scrub PII is an immense security vulnerability. This engine operates as a strict, local firewall, employing high-performance regex algorithms to deterministically eradicate emails, credit cards, SSNs, CPFs, and phone numbers. It seamlessly replaces sensitive intelligence with `[REDACTED]` tags locally, ensuring your client data remains entirely uncompromised before the LLM even sees the context.


## Available Tools (1)
- **redact_pii_strictly**: Instantly replaces Emails, CPFs, SSNs, and Credit Cards with [REDACTED] tags using fast offline regex


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Strict PII Redaction Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Execute the strict redaction engine on this contract to remove all CPFs and Emails before we send the summary to Claude."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.

---

**👤 You:**
> "We have an extensive leak log. Process it through the engine to ensure every single 16-digit credit card number is destroyed."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.

---

**👤 You:**
> "Remove all standard phone numbers and SSNs from this 50-page deposition transcript before filing it to the public record."

**🤖 AI Agent:**
> The computation has been executed with mathematical precision. All results are exact and ready for review.


## ❓ FAQ

**Q: Does it read the meaning of the text?**
No, it strictly executes compiled local mathematical regex patterns, ensuring it never hallucinates or leaks contextual data.

**Q: What data points are redacted?**
The engine strips standard email addresses, 16-digit credit cards, US SSNs, Brazilian CPFs, and generic phone number formats.

**Q: Is the original text preserved?**
The tool returns a completely sanitized clone of the document string, leaving the raw client source completely untouched locally.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/strict-pii-redaction-engine](https://vinkius.com/mcp/strict-pii-redaction-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Strict PII Redaction Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `strict-pii-redaction-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Strict PII Redaction Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "strict-pii-redaction-engine": {
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
