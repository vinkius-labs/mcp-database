# JWT Decoder & Verifier MCP Server

Decode and mathematically verify JWT tokens local. Ensure API authentication tokens are cryptographically authentic and not expired.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/jwt-decoder-verifier)

## Overview
**Category:** fort-knox
**Tools Count:** 1

## Description
While an AI Agent can base64-decode a JSON Web Token to read its claims, it is physically incapable of verifying the cryptographic signature. This means an AI could accept a forged token or an expired session without knowing. This MCP solves that by offloading the mathematical signature verification to the V8 engine.

### The Superpowers

- **Cryptographic Verification:** Uses `jsonwebtoken` to strictly verify the token signature against the provided secret key.
- **Local Decoding:** Extract user IDs, roles, and expiration dates instantly without network latency.


## Available Tools
- **decode_jwt**: Pass the JWT string and optionally a secret or public key. The engine decodes the header, payload, and validates the signature offline.

Decodes JSON Web Tokens (JWT) and mathematically verifies cryptographic signatures offline


## Installation & Usage

To install and use the **JWT Decoder & Verifier** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jwt-decoder-verifier](https://vinkius.com/mcp/jwt-decoder-verifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
