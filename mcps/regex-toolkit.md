# Regex Toolkit MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/regex-toolkit)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/regex-toolkit-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/regex-toolkit-mcp)
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


## Installation & Usage

To install and use the **Regex Toolkit** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/regex-toolkit](https://vinkius.com/mcp/regex-toolkit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
