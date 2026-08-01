# PII Redaction Deterministic Scrubber Alternative MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pii-redaction-deterministic-scrubber-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Detects and redacts SSNs, emails, phone numbers, credit cards, and IBANs using regex and checksums.

## Description
The PII Redaction Deterministic Scrubber provides a high-precision pipeline for identifying and masking Personally Identifiable Information (PII) within unstructured text. Unlike probabilistic models, this server utilizes strict regular expression patterns combined with algorithmic checksum validators, such as the Luhn algorithm for credit card verification and ABA routing number validation for financial identifiers. The `redact_pii` tool processes input strings to identify sensitive entities including Social Security Numbers (SSN), email addresses, telephone numbers, and IBANs. For every execution, the engine returns a structured result containing the redacted text, a precise count of each PII type detected, and the exact character offsets for every identified match, enabling downstream systems to audit redaction coverage without exposing sensitive data.


## Available Tools (1)
- **redact_pii**: Detects and redacts PII (SSN, Email, Phone, Credit Card, IBAN) from text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PII Redaction Deterministic Scrubber Alternative** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Redact the PII from this text: 'My email is jane.doe@vinkius.com and my credit card is 4532015112830363.'"

**🤖 AI Agent:**
> {"redactedText": "My email is [REDACTED] and my credit card is [REDACTED].", "counts": {"email": 1, "creditCard": 1}, "offsets": [{"type": "email", "start": 16, "end": 35}, {"type": "creditCard", "start": 52, "end": 68}]}

---

**👤 You:**
> "Check this IBAN for PII: 'DE89370400440532013000'"

**🤖 AI Agent:**
> {"redactedText": "[REDACTED]", "counts": {"iban": 1}, "offsets": [{"type": "iban", "start": 0, "end": 20}]}

---

**👤 You:**
> "Scan this text for SSN: 'The user's SSN is 999-00-1234.'"

**🤖 AI Agent:**
> {"redactedText": "The user's SSN is [REDACTED].", "counts": {"ssn": 1}, "offsets": [{"type": "ssn", "start": 21, "end": 33}]}


## ❓ FAQ

**Q: Does this tool use AI or Machine Learning for detection?**
No. It uses deterministic regex patterns and checksum validators like the Luhn algorithm to ensure 100% predictable results without ML overhead.

**Q: What types of PII can be redacted?**
The `redact_pii` tool detects SSNs, emails, phone numbers, credit cards (via Luhn), and IBANs.

**Q: How can I use this in my AI agent?**
You can connect via Vinkius Edge using your personal Connection Token. Once connected, you can call the `redact_pii` tool directly from Cursor, Claude Desktop, or any MCP-compatible client.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pii-redaction-deterministic-scrubber-alternative](https://vinkius.com/mcp/pii-redaction-deterministic-scrubber-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PII Redaction Deterministic Scrubber Alternative** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pii-redaction-deterministic-scrubber-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PII Redaction Deterministic Scrubber Alternative** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pii-redaction-deterministic-scrubber-alternative": {
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
