# IBAN and BIC Checksum Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/iban-and-bic-checksum-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Verify the mathematical integrity of IBANs and the structural validity of BIC/SWIFT codes.

## Description
This MCP server provides precise validation for international banking identifiers. It uses the MOD-97 algorithm to confirm the mathematical accuracy of IBANs and enforces strict alphanumeric structural rules for BIC/SWIFT codes. Use `validate_iban` to check if an IBAN is valid, `validate_bic` to verify a BIC code, or `get_validation_rules` to retrieve expected IBAN lengths for specific countries.


## Available Tools (3)
- **get_validation_rules**: Provides a list of expected IBAN lengths per country
- **validate_bic**: Determines if a string follows the strict structural rules of a BIC
- **validate_iban**: Checks if a given string is a mathematically valid IBAN


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IBAN and BIC Checksum Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is this IBAN valid: DE89370400440532013000?"

**🤖 AI Agent:**
> Yes, that is a valid IBAN for Germany.

---

**👤 You:**
> "Check if this BIC is correct: ABCDEFF1XXX"

**🤖 AI Agent:**
> Yes, the BIC code is structurally valid.

---

**👤 You:**
> "What is the expected length for an IBAN in France?"

**🤖 AI Agent:**
> The expected length for an IBAN in France is 27 characters.


## ❓ FAQ

**Q: How does the IBAN validation work?**
The `validate_iban` tool performs a MOD-97 checksum. It rearranges the IBAN, converts letters to numbers, and verifies that the remainder of the division by 97 is 1.

**Q: Can I check the length requirements for a specific country?**
Yes, you can use `get_validation_rules` to find the required character length for an IBAN in a specific country code.

**Q: What is the difference between IBAN and BIC?**
IBAN identifies a specific bank account, while BIC (or SWIFT) identifies the specific bank. You can validate both using `validate_iban` and `validate_bic` respectively.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/iban-and-bic-checksum-validator](https://vinkius.com/mcp/iban-and-bic-checksum-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **IBAN and BIC Checksum Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `iban-and-bic-checksum-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **IBAN and BIC Checksum Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "iban-and-bic-checksum-validator": {
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
