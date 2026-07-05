# Number Base Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/number-base-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Convert integers and fractional numbers between any bases from 2 to 36 with high precision.

## Description
A high-precision utility for converting numeric values between any bases from 2 to 36. This MCP server handles extremely large integers using BigInt and supports fractional numbers with configurable precision. Beyond simple conversion, it provides an educational breakdown of the mathematical process via `get_conversion_trace`, showing each division or multiplication step. You can also use `validate_alphabet_compatibility` to ensure custom symbol sets match your target base size. Perfect for developers working with binary, hex, base64-style alphabets, or any positional notation system.


## Available Tools (3)
- **convert_number**: Use precision for fractions.

Converts a number from one base to another
- **get_conversion_trace**: Generates a step-by-step conversion trace
- **validate_alphabet_compatibility**: Validates a custom alphabet for a specific base


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Number Base Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert the decimal number 255 to hexadecimal."

**🤖 AI Agent:**
> The decimal number 255 in hexadecimal is FF.

---

**👤 You:**
> "Show me the conversion steps for converting 13 from base 10 to base 2."

**🤖 AI Agent:**
> Step 1: Divide 13 by 2, remainder 1. Step 2: Divide 6 by 2, remainder 0. Step 3: Divide 3 by 2, remainder 1. Step 4: Divide 1 by 2, remainder 1. Result: 1101.

---

**👤 You:**
> "Is the alphabet 'ABC' valid for base 3?"

**🤖 AI Agent:**
> Yes, the alphabet 'ABC' is a valid sequence of 3 unique symbols for base 3.


## ❓ FAQ

**Q: What is the maximum base supported?**
The server supports any base from 2 up to 36, using the standard alphanumeric set (0-9 and A-Z).

**Q: Can I use custom symbols for my base?**
Yes, you can provide a custom alphabet string to `convert_number`. Use `validate_alphabet_compatibility` first to ensure your alphabet length matches the target base.

**Q: How does it handle very large numbers?**
The engine uses BigInt for the integer part, allowing you to process numbers with thousands of digits without any precision loss.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/number-base-converter](https://vinkius.com/mcp/number-base-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Number Base Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `number-base-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Number Base Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "number-base-converter": {
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
