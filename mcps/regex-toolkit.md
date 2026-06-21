# Regex Toolkit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/regex-toolkit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Equip your AI with strict Regular Expressions. Deterministically extract, validate, and redact Emails, URLs, and Phones without hallucinations.

## Description
Parsing unstructured text to find contact information is a classic LLM vulnerability. AI models often "guess" email boundaries or invent fake phone numbers when summarizing text. The Regex Toolkit MCP enforces strict mathematical patterns to guarantee 100% extraction and validation accuracy.

### The Superpowers
- **Flawless Extraction:** Pull every single valid Email, URL, or Phone number from a giant block of text instantly into a clean JSON array.
- **Zero-Trust Validation:** Ensure that user inputs are structurally perfect before passing them to external databases or CRMs.
- **PII Redaction Engine:** Instantly mask sensitive client data (`[EMAIL_REDACTED]`) before generating public reports or passing context to unsecure layers.
- **Privacy First (Local):** Your data never leaves your infrastructure. The regex engine compiles and executes entirely locally.


## Available Tools
- **mask_sensitive_data**: Redacts sensitive PII (emails, phones, URLs) from a text blob by replacing them with [REDACTED] tags
- **validate_pattern**: Validates if a single string perfectly matches an email, URL, or phone format
- **extract_pattern**: Extracts all unique emails, URLs, or phone numbers from a large body of text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Regex Toolkit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract all email addresses from this massive support ticket transcript."

**🤖 AI Agent:**
> Using the extract_pattern tool (type='email'): I found 3 unique emails: ['user@gmail.com', 'admin@company.net', 'billing@startup.io'].

---

**👤 You:**
> "Mask all sensitive phone numbers and emails in this document before I save it to the public database."

**🤖 AI Agent:**
> Using the mask_sensitive_data tool: The sanitized text is: 'Contact [EMAIL_REDACTED] or call [PHONE_REDACTED] for support.'

---

**👤 You:**
> "Verify if 'https://www.vinkius.com/dashboard?user=123' is a mathematically valid URL."

**🤖 AI Agent:**
> Using the validate_pattern tool (type='url'): Yes, it is a perfectly valid URL structure.


## ❓ FAQ

**Q: Why use this instead of asking the AI to find the emails?**
Because LLMs predict text probabilistically. They might miss emails embedded in weird characters (like `contact@company.com.` with a trailing dot) or hallucinate non-existent addresses. Regex provides mathematical certainty.

**Q: Does the PII masking send data to the cloud?**
Never. The `mask_sensitive_data` tool runs exclusively on your local Javascript engine (V8). It acts as a local firewall, ensuring sensitive strings are redacted before any external processing happens.

**Q: What format of phone numbers are supported?**
The regex captures international formats with country codes (e.g., +1, +55), optional parentheses for area codes, and spacing/hyphens commonly used globally.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/regex-toolkit](https://vinkius.com/mcp/regex-toolkit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Regex Toolkit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `regex-toolkit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Regex Toolkit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "regex-toolkit": {
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
