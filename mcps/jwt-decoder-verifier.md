# JWT Decoder & Verifier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jwt-decoder-verifier)
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


## ❓ FAQ

**Q: Can I decode a token without the secret?**
Yes, if you omit the secret, it will only decode the payload, but it will not verify authenticity.

**Q: Does it check expiration dates?**
Yes, if the secret is provided, it will automatically throw an error if the token is expired.

**Q: What algorithms does it support?**
It supports standard JWT algorithms including HS256, HS384, and HS512.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jwt-decoder-verifier](https://vinkius.com/mcp/jwt-decoder-verifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JWT Decoder & Verifier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `jwt-decoder-verifier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JWT Decoder & Verifier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jwt-decoder-verifier": {
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
