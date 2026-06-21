# Rong360 Open API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rong360-open-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Bring high-level financial risk assessment and identity KYC directly to your agent. Evaluate credit scores and verify names.

## Description
Connect your AI backend directly to **Rong360** (融360), a massive financial big-data hub in China. With this MCP server, your LLMs can execute deep background checks, calculate credit risk, and perform facial-KYC without implementing convoluted RSA algorithms manually.

### What you can do

- **Identity Verification** — Check if an ID number matches the provided Real Name directly with authorities
- **Credit Scoring** — Evaluate consumer loaning scores to identify defaulting behaviors instantly
- **Carrier Validation** — Confirm if a given phone number has been officially registered under the user's name

### How it works

1. Subscribe to this server
2. Insert your **App ID** and your **RSA Private Key** from the [Rong360 Open Platform](https://open.rong360.com/)
3. Start verifying consumers dynamically from the MCP console directly

### Who is this for?

- **Fintech Underwriters** — Allow agents to automatically process preliminary credit evaluations before humans review loans
- **P2P Marketplaces** — Detect scammers by verifying carrier information and matching IDs to face scans automatically
- **Security Teams** — Build robust AI vetting workflows prior to onboarding high-value accounts


## Available Tools
- **check_credit_score**: Generate a big data credit score profile
- **detect_face**: Perform facial recognition matching against a government ID
- **validate_mobile_number**: Validate carrier ownership of a mobile phone
- **verify_identity**: Verify a national ID card and real name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rong360 Open API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Verify the identity for the name 'Lu Han', ID Number 1101051990XXXXXXXX."

**🤖 AI Agent:**
> I've checked the KYC registry. The real name matches the ID card number perfectly.

---

**👤 You:**
> "Generate a credit score report for phone 13912345678 and ID 310115XXXX."

**🤖 AI Agent:**
> The Rong360 credit system returns a score of 620. No loan defaulting history was detected, but multiple micro-loan inquiries were made in the last 30 days.


## ❓ FAQ

**Q: How is the RSA signature handled?**
Rong360 APIs typically require generating a strict base64 signature for each URL. This MCP server entirely abstracts that operation. You just securely paste your pkcs8 Private Key once during setup, and the agentic execution environment automatically handles URL signing on each outgoing LLM request.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rong360-open-api](https://vinkius.com/mcp/rong360-open-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rong360 Open API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `rong360-open-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rong360 Open API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rong360-open-api": {
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
