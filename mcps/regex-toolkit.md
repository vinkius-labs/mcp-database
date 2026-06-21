# Regex Toolkit MCP Server

Equip your AI with strict Regular Expressions. Deterministically extract, validate, and redact Emails, URLs, and Phones without hallucinations.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/regex-toolkit)

## Overview
**Category:** developer-tools
**Tools Count:** 3

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


## Installation & Usage

To install and use the **Regex Toolkit** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/regex-toolkit](https://vinkius.com/mcp/regex-toolkit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
