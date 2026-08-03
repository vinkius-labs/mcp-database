# JWT Payload Extractor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jwt-payload-extractor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Extract and decode JWT payloads deterministically without cryptographic verification.

## Description
The `jwt-payload-extractor` implements a deterministic decoding pipeline for inspecting JSON Web Token (JWT) payloads without cryptographic verification. The process begins by splitting the input string via the period delimiter to isolate the second segment. It then performs Base64URL normalization, specifically replacing hyphens (`-`) with plus signs (`+`) and underscores (`_`) with forward slashes (`/`), before applying standard Base64 decoding via `atob`. This allows for the extraction of claims such as 'sub', 'iat', or custom identifiers. The server also facilitates temporal analysis by parsing the 'exp' claim and comparing its Unix timestamp against the current system clock to determine token validity.

### Available Tools

`decode_jwt_payload`, `check_token_expiry`, `extract_token_identity`


## Available Tools (3)
- **extract_token_identity**: Extracts a specific identity claim from a JWT token
- **check_token_expiry**: Checks the expiration of a JWT token
- **decode_jwt_payload**: Decodes the payload of a JWT string


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JWT Payload Extractor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Decode this JWT and tell me what the payload contains: [REDACTED]"

**🤖 AI Agent:**
> { "sub": "1234567890", "name": "John Doe", "iat": 1516239022 }

---

**👤 You:**
> "Is this token expired? [REDACTED]"

**🤖 AI Agent:**
> The expiration timestamp is 1516239022. Based on the current time, the token is expired.

---

**👤 You:**
> "Extract the 'user_role' from this token: [REDACTED]"

**🤖 AI Agent:**
> The value for the 'user_role' key is 'admin'.


## ❓ FAQ

**Q: Does this tool verify the JWT signature?**
No, the server focuses exclusively on the deterministic parsing of the payload segment. It does not utilize any cryptographic primitives or secret keys to validate the integrity of the signature segment. Tools available: `decode_jwt_payload`, `check_token_expiry`, `extract_token_identity`.

**Q: How can I see the expiration date of a token?**
The server extracts the 'exp' claim from the decoded JSON object and compares its Unix timestamp against the current system time to identify if the token's operational window has expired.

**Q: Can I extract specific user IDs from the token?**
Yes. After parsing the payload segment into a JSON structure, the server traverses the object hierarchy to retrieve the value associated with any specified key, such as 'sub' or custom user identifiers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jwt-payload-extractor](https://vinkius.com/mcp/jwt-payload-extractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JWT Payload Extractor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jwt-payload-extractor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JWT Payload Extractor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jwt-payload-extractor": {
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
