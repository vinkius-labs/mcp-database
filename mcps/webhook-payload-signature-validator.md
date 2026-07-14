# Webhook Payload Signature Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/webhook-payload-signature-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Validate inbound webhook authenticity using HMAC signature verification and timestamp freshness checks.

## Description
The Webhook Payload Signature Validator provides a secure way to verify the integrity and temporal validity of incoming webhooks. By utilizing tools like `identify_signature_scheme`, `verify_hmac_standard`, and `verify_hmac_timestamped`, you can protect your systems against tampering, replay attacks, and timing analysis. It supports common formats such as GitHub's static signatures and Stripe-style timestamped headers.


## Available Tools (3)
- **verify_hmac_standard**: Requires the raw payload and the shared secret.

Verify a webhook signature using the standard HMAC-SHA256 method
- **identify_signature_scheme**: Useful before attempting verification.

Identify the webhook signature verification strategy
- **verify_hmac_timestamped**: " and "v1=...". This prevents replay attacks by checking the timestamp drift.

Verify a webhook signature using the timestamped HMAC-SHA256 method


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Webhook Payload Signature Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Identify the scheme for this header: 't=1625097600,v1=abc'"

**🤖 AI Agent:**
> The detected scheme is TIMESTAMPED.

---

**👤 You:**
> "Verify this GitHub webhook payload with secret 'my_secret' and signature '5d41402abc4b2a76b9719d911017c592'."

**🤖 AI Agent:**
> The signature is valid.

---

**👤 You:**
> "Is this Stripe-style header from 10 minutes ago still valid if my max drift is 5 minutes?"

**🤖 AI Agent:**
> No, the timestamp has expired.


## ❓ FAQ

**Q: How does the tool prevent replay attacks?**
By using `verify_hmac_timestamped`, the system checks if the timestamp in the header is within the allowed drift window.

**Q: What signature formats are supported?**
It supports static signatures like GitHub's and timestamped signatures like Stripe's.

**Q: Does it protect against timing attacks?**
Yes, the implementation uses constant-time comparison to mitigate timing analysis risks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/webhook-payload-signature-validator](https://vinkius.com/mcp/webhook-payload-signature-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Webhook Payload Signature Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `webhook-payload-signature-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Webhook Payload Signature Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "webhook-payload-signature-validator": {
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
