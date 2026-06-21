# Phone Validator Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/phone-validator-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Stop LLMs from hallucinating phone numbers. Validates and formats numbers to E.164 natively.

## Description
LLMs often accept chaotic phone number inputs or try to format them incorrectly before sending to Twilio or Zenvia. This MCP brings Google's libphonenumber-js to the Edge.

### The Superpowers

- **E.164 Strict Format:** Cleans and formats chaotic inputs into mathematically perfect E.164 strings.
- **Country Validation:** Validates the exact country code and identifies fake numbers immediately.


## Available Tools
- **validate_phone**: Pass the raw phone string and optionally a country code. The engine uses libphonenumber to validate structure, detect carrier type, and format to E.164 standard.

Validates and formats a phone number deterministically to E.164 standard using Google libphonenumber-js


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Phone Validator Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Clean and format this messy user input into an E.164 phone number: '+44 (0) 20 7946 0958'"

**🤖 AI Agent:**
> ✅ **Result:** Perfectly mapped to E.164 format: `+442079460958`

---

**👤 You:**
> "Check if the input `11 98888-0000` is structurally valid, assuming the default country is Brazil (`BR`)."

**🤖 AI Agent:**
> ✅ **Validation Status:** Valid.
- **Country:** `BR`
- **E.164:** `+5511988880000`

---

**👤 You:**
> "Extract the Alpha-2 Country Code from this international number: `+1-415-555-2671`."

**🤖 AI Agent:**
> ✅ **Country Identified:** The number strictly belongs to `US` (United States).


## ❓ FAQ

**Q: Does it support Brazilian numbers?**
Yes, perfectly handles the 9-digit rule.

**Q: Can it extract the country?**
Yes, it returns the Alpha-2 country code.

**Q: Is it local?**
Yes, 100% local regex/metadata evaluation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/phone-validator-engine](https://vinkius.com/mcp/phone-validator-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Phone Validator Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `phone-validator-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Phone Validator Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "phone-validator-engine": {
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
