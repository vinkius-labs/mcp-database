# SMS GSM-7 Sanitizer MCP Server

Stop telecom bill shocks. Strip emojis and complex Unicode to guarantee 100% GSM-7 SMS compatibility and prevent multi-part charges.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sms-gsm-7-sanitizer)

## Overview
**Category:** developer-tools
**Tools Count:** 1

## Description
When a Martech AI Agent drafts an SMS campaign via Twilio or Zenvia, the LLM will often include emojis (🚀) or smart quotes (`”` instead of `"`). This instantly breaks the standard 160-character GSM-7 encoding, reducing the limit to 70 characters and splitting the message into 3 parts. The client ends up paying 3x more for the campaign. This MCP solves that perfectly.

### The Superpowers

- **Emoji Eradication:** Safely strips all emojis and zero-width characters using aggressive regular expressions.
- **Unicode Transliteration:** Converts complex accents and symbols into safe 7-bit ASCII (GSM-7) to guarantee maximum character limits per message segment.


## Available Tools
- **sanitize_gsm7**: Pass the draft text and the engine will strip emojis and transliterate Unicode to pure 7-bit ASCII, guaranteeing GSM-7 encoding and maximum 160-character segments.

Strips emojis and complex Unicode to guarantee 100% GSM-7 compatibility. Prevents Twilio from charging 3x for multi-part SMS messages


## Installation & Usage

To install and use the **SMS GSM-7 Sanitizer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sms-gsm-7-sanitizer](https://vinkius.com/mcp/sms-gsm-7-sanitizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
