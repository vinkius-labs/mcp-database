# IBAN Bank Validator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/iban-bank-validator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/iban-bank-validator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/iban-bank-validator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Validate international bank accounts instantly using Modulus 97 checksums. Prevent failed transactions with 100% local precision.

## Description
Validating an IBAN (International Bank Account Number) requires executing Modulus 97 arithmetic across a 34-character string. LLMs are incapable of performing this math, often guessing validity and causing failed international payouts in platforms like Wise or Stripe. This MCP brings strict banking validation to the edge.

### The Superpowers

- **Modulus 97 Math:** Performs exact mathematical checksum validation local.
- **Format Check:** Verifies exact country-specific lengths and alphanumeric patterns before processing.


## Available Tools
- **validate_iban**: Pass the full IBAN string and the engine performs the Modulus 97 checksum calculation to verify structural and mathematical validity.

Validates international bank account numbers (IBAN) using mathematical Modulus 97 checksum


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IBAN Bank Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Run the Modulus 97 math to verify if this European IBAN `GB82WEST12345698765432` is valid before we initiate the transfer."

**🤖 AI Agent:**
> ✅ **Validation Passed:** The IBAN checksum is mathematically correct and matches the GB length requirements.

---

**👤 You:**
> "Extract the country code and sanitize this messy user input: ` FR 14 2004 1010 0505 0001 3M02 606 `."

**🤖 AI Agent:**
> ✅ **Sanitized:** `FR1420041010050500013M02606`
- **Country:** `FR` (France)
- **Validity:** True

---

**👤 You:**
> "Ensure this IBAN `DE89370400440532013000` is structurally perfect."

**🤖 AI Agent:**
> ✅ **Status:** Valid.


## Installation & Usage

To install and use the **IBAN Bank Validator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/iban-bank-validator](https://vinkius.com/mcp/iban-bank-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
