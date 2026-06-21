# Bcrypt Hash Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bcrypt-hash-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Hash and verify passwords with the industry-standard bcrypt algorithm. Two tools in one: hash with configurable salt rounds, and verify against stored hashes. Pure JS — zero compilation.

## Description
An agent just generated a user registration flow. The password is stored in plaintext. That's not a bug — it's a security incident waiting to happen.

Bcrypt is the algorithm that Dropbox, GitHub, and every serious authentication system uses for password storage. It includes a built-in salt, is intentionally slow to resist brute-force, and this MCP provides it as pure JavaScript — no native compilation, no node-gyp headaches.

### The Superpowers

- **Two Tools, One MCP:** `bcrypt_hash` creates the hash, `bcrypt_verify` checks passwords against stored hashes.
- **Built-in Salt:** Every hash includes a unique random salt — no manual salt management needed.
- **Configurable Cost:** Salt rounds 4-16. Default 10 (~100ms). 12 for financial systems. 14+ for government.
- **Pure JavaScript:** Uses bcryptjs — works in Edge, Lambda, Cloudflare Workers, and any Node.js runtime without compilation.


## Available Tools (2)
- **bcrypt_hash**: Bcrypt is the industry standard for password hashing — it includes a salt and is intentionally slow to resist brute-force attacks. Salt rounds control the computational cost (10 is default, 12+ for high security). Never store plaintext passwords.

Hashes a password using bcrypt with configurable salt rounds. Pure JS, no native compilation needed
- **bcrypt_verify**: Pass the password and the hash, and receive a boolean isMatch result. This is the only correct way to verify bcrypt passwords — never compare hashes directly.

Verifies a password against a bcrypt hash. Returns boolean match result


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bcrypt Hash Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "A new user just signed up. Hash their password 'MyS3cur3P@ss!' for secure storage in PostgreSQL."

**🤖 AI Agent:**
> Hash: $2a$10$N9qo8uLOickgx2ZMRZoMye... | 60 chars, salt embedded, ready for INSERT.

---

**👤 You:**
> "User is trying to log in. Check if their password matches the stored hash."

**🤖 AI Agent:**
> isMatch: true — password verified. Allow login.

---

**👤 You:**
> "Our compliance officer requires 12 salt rounds minimum. Re-hash this password with higher security."

**🤖 AI Agent:**
> Hash: $2a$12$... | 12 rounds, ~400ms computation time. Meets financial-grade requirements.


## ❓ FAQ

**Q: Why bcrypt instead of SHA-256 or MD5 for passwords?**
SHA-256 and MD5 are fast — that's the problem. An attacker can try billions of hashes per second. Bcrypt is intentionally slow (configurable via salt rounds), making brute-force attacks economically infeasible.

**Q: What salt rounds should I use for a financial application?**
12 minimum. Each additional round doubles the computation time. 10 = ~100ms, 12 = ~400ms, 14 = ~1.6s. Balance security vs. login latency for your use case.

**Q: Can I verify a password without knowing the salt?**
Yes — that's the beauty of bcrypt. The salt is embedded in the hash string itself ($2a$10$...). Just pass the password and the stored hash to bcrypt_verify.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bcrypt-hash-engine](https://vinkius.com/mcp/bcrypt-hash-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bcrypt Hash Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bcrypt-hash-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bcrypt Hash Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bcrypt-hash-engine": {
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
