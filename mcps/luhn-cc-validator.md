# Luhn CC Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/luhn-cc-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Stop LLMs from sending fake credit card numbers to payment gateways. Validates the mathematical Luhn check instantly.

## Description
LLMs cannot perform complex algorithmic validation like the Luhn check. This results in agents trying to process fake or mistyped credit card numbers, burning API limits and triggering anti-fraud systems. This MCP adds pure, zero-latency validation to the edge.

### The Superpowers

- **Pre-Flight Validation:** Instantly block mathematically invalid credit card numbers before making costly Stripe/Adyen API calls.
- **Brand Detection:** Accurately identifies Visa, Mastercard, AMEX, and Discover purely based on mathematical prefixes.


## Available Tools
- **validate_luhn**: Pass the card number string and receive validation status plus card brand detection (Visa, Mastercard, Amex).

Validates credit card numbers using the mathematical Luhn algorithm and detects the card brand


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Luhn CC Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Run the Luhn algorithm to check if `4242424242424242` is a mathematically valid credit card number."

**🤖 AI Agent:**
> ✅ **Checksum Valid:** Passed Luhn verification. Brand identified as `Visa` based on prefix rules.

---

**👤 You:**
> "A user submitted `378282246310005`. Verify the checksum and detect if it is American Express."

**🤖 AI Agent:**
> ✅ **Validation Status:** Valid.
- **Brand:** `American Express`
- **Sanitized:** Cleaned spaces and hyphens successfully.

---

**👤 You:**
> "Validate this mistyped card number `5555444433332221` before sending it to the Stripe API."

**🤖 AI Agent:**
> ❌ **Pre-flight Error:** Blocked! The number failed the mathematical Luhn modulo-10 checksum.


## ❓ FAQ

**Q: Does it process payments?**
No, it purely validates the mathematical checksum of the number. It does not contact any bank.

**Q: Is it secure?**
Yes, 100% local evaluation inside the edge worker memory. No network requests are made.

**Q: What brands are supported?**
Visa, Mastercard, American Express, and Discover are instantly identified.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/luhn-cc-validator](https://vinkius.com/mcp/luhn-cc-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Luhn CC Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `luhn-cc-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Luhn CC Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "luhn-cc-validator": {
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
