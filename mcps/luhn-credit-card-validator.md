# Luhn Credit Card Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/luhn-credit-card-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Validates credit card numbers using the Luhn algorithm and identifies the issuer.

## Description
This MCP server provides tools to verify the mathematical validity of credit card numbers using the Luhn mod-10 algorithm. It can identify card issuers such as Visa, Mastercard, and American Express by analyzing digit patterns and lengths. Use `validate_card_number` for a full check of validity and issuer, `identify_issuer_only` to find the network without a checksum, or `get_issuer_rules` to see the specific prefix and length requirements for a known issuer.


## Available Tools (3)
- **get_issuer_rules**: Answers what the specific length and prefix requirements are for recognized card issuers
- **identify_issuer_only**: Answers what specific card network a number belongs to without performing the full Luhn mathematical validation
- **validate_card_number**: Answers whether a specific credit card number is mathematically valid and which issuer it belongs to


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Luhn Credit Card Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is the credit card number 4539 1234 5678 9012 valid?"

**🤖 AI Agent:**
> Yes, the card number is a valid Visa card.

---

**👤 You:**
> "What issuer is card number 3712 345678 90123?"

**🤖 AI Agent:**
> That card number belongs to American Express.

---

**👤 You:**
> "Check if 5105 1051 0510 5105 is a valid Mastercard."

**🤖 AI Agent:**
> No, that number is not a valid Mastercard.


## ❓ FAQ

**Q: How does the validation work?**
The server uses the Luhn mod-10 algorithm to perform a checksum on the digits, ensuring the number is mathematically consistent with standard credit card formats.

**Q: Which card issuers are supported?**
The tool currently identifies Visa, Mastercard, and American Express.

**Q: Can I use this to check if a card is active?**
No, this tool only validates the mathematical structure of the number. It cannot check if a card is active, has funds, or is stolen.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/luhn-credit-card-validator](https://vinkius.com/ai-agent-connect/luhn-credit-card-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Luhn Credit Card Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `luhn-credit-card-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Luhn Credit Card Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "luhn-credit-card-validator": {
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
