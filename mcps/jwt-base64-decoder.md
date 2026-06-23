# JWT & Base64 Decoder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jwt-base64-decoder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Stop hallucinating Base64 translations. Instantly decode complex JWT tokens into readable headers and payloads with exact expiration mathematics.

## Description
Decode Base64 strings and JWT tokens with exact binary precision using native Node buffers. Never let an LLM guess an expiration date again.


## Available Tools (2)
- **decode_base64_string**: Pass the raw JWT string and receive the parsed JSON without any signature verification.

Decodes any Base64 string deterministically into UTF-8 text
- **decode_jwt_token**: Pass the raw Base64 text and receive the decoded content.

Decodes a JWT token deterministically. Extracts the header, payload, and calculates the exact expiration date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JWT & Base64 Decoder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Decode this Authorization Bearer JWT safely to extract the 'sub' and 'exp' claims."

**🤖 AI Agent:**
> ✅ **Decoded Payload:**
```json
{
  "sub": "usr_88129a",
  "exp": 1731945600
}
```

---

**👤 You:**
> "Evaluate if the expiration timestamp in this decoded JWT is in the past."

**🤖 AI Agent:**
> ✅ **Status:** Token is expired. The `exp` claim translates to 2023-11-05.

---

**👤 You:**
> "Decode this raw Base64 string payload returned by the external API."

**🤖 AI Agent:**
> ✅ **Base64 Decoded:** Returned plain UTF-8 text representation.


## ❓ FAQ

**Q: Is it secure?**
Yes, decoding runs completely local.

**Q: Does it verify the JWT signature?**
No, this is a strict decoder for reading payloads, not an authentication gateway.

**Q: Can it decode hex as well?**
It is specialized in Base64 and JWT headers/payloads.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jwt-base64-decoder](https://vinkius.com/mcp/jwt-base64-decoder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JWT & Base64 Decoder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jwt-base64-decoder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JWT & Base64 Decoder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jwt-base64-decoder": {
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
