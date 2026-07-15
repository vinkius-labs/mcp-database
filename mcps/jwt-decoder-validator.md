# JWT Decoder & Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jwt-decoder-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Decode JWT segments and verify cryptographic signatures and temporal claims.

## Description
This MCP server provides a specialized utility to inspect JSON Web Tokens (JWT). You can use `parse_jwt_string` to check the structural integrity of a token, `decode_jwt_components` to extract readable JSON from headers and payloads, `verify_jwt_signature` to cryptographically validate signatures using HS256, RS256, or ES256 algorithms, and `validate_jwt_temporal_claims` to ensure tokens are not expired or active before their 'nbf' time.


## Available Tools (4)
- **verify_jwt_signature**: Cryptographically validates that the signature matches the provided header and payload using a specified key
- **decode_jwt_components**: Extracts and decodes the readable JSON content from the JWT header and payload
- **parse_jwt_string**: Verifies if a provided string adheres to the fundamental three-part format of a JWT
- **validate_jwt_temporal_claims**: Checks the validity of standard time-based claims against the current system time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JWT Decoder & Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is this JWT valid: eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ.SflKxwRJSMeKKF2QT4fwpMeJf36POk6yJV_adQssw5c"

**🤖 AI Agent:**
> The token structure is valid, and the `parse_jwt_string` tool confirms it contains 3 segments.

---

**👤 You:**
> "Decode this JWT payload: eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ"

**🤖 AI Agent:**
> The decoded payload is: {"sub":"1234567890","name":"John Doe","iat":1516239022}

---

**👤 You:**
> "Check if this payload is still valid at timestamp 1700000000: {"exp": 1600000000}"

**🤖 AI Agent:**
> The token is not temporally valid because the 'exp' claim has passed.


## ❓ FAQ

**Q: What algorithms are supported for signature verification?**
The `verify_jwt_signature` tool supports HS256, RS256, and ES256 algorithms.

**Q: Can I check if a token has expired?**
Yes, by using the `validate_jwt_temporal_claims` tool with the decoded payload and the current timestamp.

**Q: Does this server verify the authenticity of the token?**
The `verify_jwt_signature` tool can validate the signature if you provide the appropriate secret or public key.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jwt-decoder-validator](https://vinkius.com/mcp/jwt-decoder-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JWT Decoder & Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jwt-decoder-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JWT Decoder & Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jwt-decoder-validator": {
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
