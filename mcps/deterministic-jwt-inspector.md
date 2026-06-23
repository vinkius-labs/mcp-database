# Deterministic JWT Inspector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deterministic-jwt-inspector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Transform your AI into a cybersecurity diagnostic tool. Instantly decode and inspect JSON Web Tokens (Headers, Payloads, and Expiry metadata) without requiring signature keys.

## Description
Debugging authentication pipelines often requires pasting sensitive JSON Web Tokens (JWTs) into public websites like jwt.io, creating severe security risks. The JWT Inspector MCP solves this by empowering your AI agent to decode and inspect authentication tokens algorithmically from within its own secure runtime.

### The Superpowers
- **Deep Payload Extraction:** Automatically decodes Base64Url segments, revealing hidden user claims, roles, and session data directly to the agent's context.
- **Automated Expiry Diagnostics:** Instantly calculates the `exp` and `iat` timestamps, comparing them against the exact current UTC time to alert the AI if the token is already expired.
- **Signature Bypassing:** Built purely for architectural debugging. It unpacks the structure without requiring public/private RSA keys, making it universally applicable for frontend and backend analysis.
- **Zero-Dependency Architecture:** Pure JS runtime execution guarantees absolute microsecond speed without pulling heavy external cryptographic libraries.


## Available Tools (1)
- **inspect_jwt**: It does not verify the signature, so do not use it to authenticate the token, only to inspect its payload and headers.

Deeply inspects and decodes a JSON Web Token (JWT), extracting the Header, Payload claims, and calculating expiry metadata without requesting verification keys


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Deterministic JWT Inspector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you inspect this JWT and tell me the user's roles? eyJ..."

**🤖 AI Agent:**
> Using the inspect_jwt tool: The decoded payload reveals the user has the roles ['admin', 'editor'].

---

**👤 You:**
> "Why is my API request failing? Is this token expired?"

**🤖 AI Agent:**
> Using the inspect_jwt tool: Yes, the metadata diagnostic shows `isExpired: true`. The token expired at 2026-05-15T12:00:00Z.

---

**👤 You:**
> "What encryption algorithm is this token using?"

**🤖 AI Agent:**
> Using the inspect_jwt tool: The header analysis indicates the token is using the 'RS256' algorithm.


## ❓ FAQ

**Q: Does this tool verify the JWT signature for authentication?**
No. The JWT Inspector is strictly a structural diagnostic tool. It bypasses signature verification to allow the AI to inspect payloads and headers during development and debugging workflows. It should not be used as a backend authentication gate.

**Q: Is it secure to decode tokens this way?**
Extremely secure. Instead of pasting your token into a third-party website, the decoding happens entirely within the deterministic V8 engine of your local agent runtime, ensuring zero data leakage.

**Q: Can it tell me if a token has expired?**
Yes. The engine automatically parses the `exp` (expiration) and `iat` (issued at) claims, converting them from UNIX timestamps into human-readable ISO dates and returning a boolean flag indicating if it is expired.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deterministic-jwt-inspector](https://vinkius.com/mcp/deterministic-jwt-inspector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Deterministic JWT Inspector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `deterministic-jwt-inspector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Deterministic JWT Inspector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deterministic-jwt-inspector": {
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
