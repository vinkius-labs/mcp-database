# JWT Decoder & Verifier MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jwt-decoder-verifier)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/jwt-decoder-verifier-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/jwt-decoder-verifier-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Decode and mathematically verify JWT tokens local. Ensure API authentication tokens are cryptographically authentic and not expired.

## Description
While an AI Agent can base64-decode a JSON Web Token to read its claims, it is physically incapable of verifying the cryptographic signature. This means an AI could accept a forged token or an expired session without knowing. This MCP solves that by offloading the mathematical signature verification to the V8 engine.

### The Superpowers

- **Cryptographic Verification:** Uses `jsonwebtoken` to strictly verify the token signature against the provided secret key.
- **Local Decoding:** Extract user IDs, roles, and expiration dates instantly without network latency.


## Available Tools
- **decode_jwt**: Pass the JWT string and optionally a secret or public key. The engine decodes the header, payload, and validates the signature offline.

Decodes JSON Web Tokens (JWT) and mathematically verifies cryptographic signatures offline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JWT Decoder & Verifier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Decode this JWT token to see what user ID is inside it."

**🤖 AI Agent:**
> JWT Payload: Decoded successfully. User ID is 123.

---

**👤 You:**
> "Verify this API JWT token using our master secret key."

**🤖 AI Agent:**
> JWT Result: Cryptographic signature verified successfully.

---

**👤 You:**
> "Check if this authentication token is expired."

**🤖 AI Agent:**
> JWT Error: TokenExpiredError: jwt expired at 2026-01-01.


## Installation & Usage

To install and use the **JWT Decoder & Verifier** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jwt-decoder-verifier](https://vinkius.com/mcp/jwt-decoder-verifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
