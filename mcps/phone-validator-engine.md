# Phone Validator Engine MCP Server

Stop LLMs from hallucinating phone numbers. Validates and formats numbers to E.164 natively.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/phone-validator-engine)

## Overview
**Category:** developer-tools
**Tools Count:** 1

## Description
LLMs often accept chaotic phone number inputs or try to format them incorrectly before sending to Twilio or Zenvia. This MCP brings Google's libphonenumber-js to the Edge.

### The Superpowers

- **E.164 Strict Format:** Cleans and formats chaotic inputs into mathematically perfect E.164 strings.
- **Country Validation:** Validates the exact country code and identifies fake numbers immediately.


## Available Tools
- **validate_phone**: Pass the raw phone string and optionally a country code. The engine uses libphonenumber to validate structure, detect carrier type, and format to E.164 standard.

Validates and formats a phone number deterministically to E.164 standard using Google libphonenumber-js


## Installation & Usage

To install and use the **Phone Validator Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/phone-validator-engine](https://vinkius.com/mcp/phone-validator-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
