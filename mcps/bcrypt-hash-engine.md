# Bcrypt Hash Engine MCP Server

Hash and verify passwords with the industry-standard bcrypt algorithm. Two tools in one: hash with configurable salt rounds, and verify against stored hashes. Pure JS — zero compilation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/bcrypt-hash-engine)

## Overview
**Category:** security
**Tools Count:** 2

## Description
An agent just generated a user registration flow. The password is stored in plaintext. That's not a bug — it's a security incident waiting to happen.

Bcrypt is the algorithm that Dropbox, GitHub, and every serious authentication system uses for password storage. It includes a built-in salt, is intentionally slow to resist brute-force, and this MCP provides it as pure JavaScript — no native compilation, no node-gyp headaches.

### The Superpowers

- **Two Tools, One MCP:** `bcrypt_hash` creates the hash, `bcrypt_verify` checks passwords against stored hashes.
- **Built-in Salt:** Every hash includes a unique random salt — no manual salt management needed.
- **Configurable Cost:** Salt rounds 4-16. Default 10 (~100ms). 12 for financial systems. 14+ for government.
- **Pure JavaScript:** Uses bcryptjs — works in Edge, Lambda, Cloudflare Workers, and any Node.js runtime without compilation.


## Available Tools
- **bcrypt_hash**: Bcrypt is the industry standard for password hashing — it includes a salt and is intentionally slow to resist brute-force attacks. Salt rounds control the computational cost (10 is default, 12+ for high security). Never store plaintext passwords.

Hashes a password using bcrypt with configurable salt rounds. Pure JS, no native compilation needed
- **bcrypt_verify**: Pass the password and the hash, and receive a boolean isMatch result. This is the only correct way to verify bcrypt passwords — never compare hashes directly.

Verifies a password against a bcrypt hash. Returns boolean match result


## Installation & Usage

To install and use the **Bcrypt Hash Engine** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bcrypt-hash-engine](https://vinkius.com/mcp/bcrypt-hash-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
