# SMS GSM-7 Sanitizer MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sms-gsm-7-sanitizer)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sms-gsm-7-sanitizer-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sms-gsm-7-sanitizer-mcp)
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


## Installation & Usage

To install and use the **SMS GSM-7 Sanitizer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sms-gsm-7-sanitizer](https://vinkius.com/mcp/sms-gsm-7-sanitizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
