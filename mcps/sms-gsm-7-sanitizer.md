# SMS GSM-7 Sanitizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sms-gsm-7-sanitizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Stop telecom bill shocks. Strip emojis and complex Unicode to guarantee 100% GSM-7 SMS compatibility and prevent multi-part charges.

## Description
When a Martech AI Agent drafts an SMS campaign via Twilio or Zenvia, the LLM will often include emojis (🚀) or smart quotes (`”` instead of `"`). This instantly breaks the standard 160-character GSM-7 encoding, reducing the limit to 70 characters and splitting the message into 3 parts. The client ends up paying 3x more for the campaign. This MCP solves that perfectly.

### The Superpowers

- **Emoji Eradication:** Safely strips all emojis and zero-width characters using aggressive regular expressions.
- **Unicode Transliteration:** Converts complex accents and symbols into safe 7-bit ASCII (GSM-7) to guarantee maximum character limits per message segment.


## Available Tools
- **sanitize_gsm7**: Pass the draft text and the engine will strip emojis and transliterate Unicode to pure 7-bit ASCII, guaranteeing GSM-7 encoding and maximum 160-character segments.

Strips emojis and complex Unicode to guarantee 100% GSM-7 compatibility. Prevents Twilio from charging 3x for multi-part SMS messages


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SMS GSM-7 Sanitizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Sanitize this SMS draft: `Hey John! 🚀 Your order is on the way. The "coffee" is hot!`"

**🤖 AI Agent:**
> SMS GSM-7 Sanitization: `Hey John! Your order is on the way. The "coffee" is hot!`

---

**👤 You:**
> "Strip all Unicode from this alert message before I send it to Twilio."

**🤖 AI Agent:**
> SMS GSM-7 Sanitization: Message is safe to send.

---

**👤 You:**
> "Make sure this marketing broadcast is strictly 7-bit ASCII."

**🤖 AI Agent:**
> SMS GSM-7 Sanitization: Sanitization applied.


## ❓ FAQ

**Q: Why does an emoji cost more?**
Emojis force the telecom provider to use UCS-2 encoding, which cuts the character limit from 160 down to 70 per message segment.

**Q: What happens to accented letters?**
Using the `unidecode` algorithm, letters like 'ç' become 'c' and 'ã' become 'a', ensuring strict ASCII compatibility.

**Q: Is this needed for WhatsApp?**
No, WhatsApp handles Unicode perfectly. This is specifically for legacy SMS gateways like Twilio and SNS.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sms-gsm-7-sanitizer](https://vinkius.com/mcp/sms-gsm-7-sanitizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SMS GSM-7 Sanitizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `sms-gsm-7-sanitizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SMS GSM-7 Sanitizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sms-gsm-7-sanitizer": {
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
