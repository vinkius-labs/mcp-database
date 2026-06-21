# IBAN Bank Validator MCP Server

Validate international bank accounts instantly using Modulus 97 checksums. Prevent failed transactions with 100% local precision.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/iban-bank-validator)

## Overview
**Category:** developer-tools
**Tools Count:** 1

## Description
Validating an IBAN (International Bank Account Number) requires executing Modulus 97 arithmetic across a 34-character string. LLMs are incapable of performing this math, often guessing validity and causing failed international payouts in platforms like Wise or Stripe. This MCP brings strict banking validation to the edge.

### The Superpowers

- **Modulus 97 Math:** Performs exact mathematical checksum validation local.
- **Format Check:** Verifies exact country-specific lengths and alphanumeric patterns before processing.


## Available Tools
- **validate_iban**: Pass the full IBAN string and the engine performs the Modulus 97 checksum calculation to verify structural and mathematical validity.

Validates international bank account numbers (IBAN) using mathematical Modulus 97 checksum


## Installation & Usage

To install and use the **IBAN Bank Validator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/iban-bank-validator](https://vinkius.com/mcp/iban-bank-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
