# IBAN Bank Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/iban-bank-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Validate international bank accounts instantly using Modulus 97 checksums. Prevent failed transactions with 100% local precision.

## Description
Validating an IBAN (International Bank Account Number) requires executing Modulus 97 arithmetic across a 34-character string. LLMs are incapable of performing this math, often guessing validity and causing failed international payouts in platforms like Wise or Stripe. This MCP brings strict banking validation to the edge.

### The Superpowers

- **Modulus 97 Math:** Performs exact mathematical checksum validation local.
- **Format Check:** Verifies exact country-specific lengths and alphanumeric patterns before processing.


## Available Tools (1)
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


## ❓ FAQ

**Q: Does it connect to banks?**
No, it purely validates the mathematical checksum of the IBAN structure.

**Q: Is it secure?**
Yes, 100% local evaluation. No data is transmitted.

**Q: What countries are supported?**
All official SEPA and international countries that use the standard IBAN format.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/iban-bank-validator](https://vinkius.com/mcp/iban-bank-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **IBAN Bank Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `iban-bank-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **IBAN Bank Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "iban-bank-validator": {
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
