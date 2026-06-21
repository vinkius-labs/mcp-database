# Sumsub MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sumsub)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Automate identity verification (KYC/AML) via Sumsub — create applicants, check verification status, and manage documents directly from any AI agent.

## Description
Connect your **Sumsub** account to any AI agent to streamline your identity verification and compliance workflows through natural conversation.

### What you can do

- **Applicant Management** — Create new applicants for KYC/AML verification levels and retrieve full profile data using unique IDs.
- **Status Tracking** — Monitor the real-time verification status of any applicant to ensure compliance requirements are met.
- **Document Handling** — Upload identity documents (passports, ID cards) directly to an applicant's profile using base64 encoding.
- **WebSDK Integration** — Generate secure access tokens to initialize the Sumsub WebSDK for your end-users seamlessly.

### How it works

1. Subscribe to this server
2. Enter your Sumsub App Token and Secret Key
3. Start managing your compliance and onboarding flows from Claude, Cursor, or any MCP-compatible client

No more manual status checks in the dashboard. Your AI acts as a compliance assistant, handling the technical heavy lifting of the Sumsub API.

### Who is this for?

- **Compliance Officers** — quickly check applicant statuses and verification details without leaving your workspace.
- **Fintech Developers** — test and manage applicant creation and token generation directly from your IDE.
- **Operations Teams** — automate the collection and processing of identity documents for faster onboarding.


## Available Tools
- **add_document**: Upload a document for an applicant
- **create_applicant**: Create a new Sumsub applicant
- **generate_access_token**: Generate WebSDK access token
- **get_applicant_status**: Get applicant verification status
- **get_applicant**: Get applicant data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sumsub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new Sumsub applicant for user 'ext_user_99' at the 'basic-kyc' level."

**🤖 AI Agent:**
> I've created the applicant. The Sumsub Applicant ID is '65b2f...a1'. You can now proceed with document uploads or status checks for this user.

---

**👤 You:**
> "Check the verification status for applicant ID 65b2f8e9c1234567890."

**🤖 AI Agent:**
> The applicant '65b2f8e9c1234567890' is currently in the 'pending' state. Sumsub is reviewing the submitted documents.

---

**👤 You:**
> "Generate a WebSDK access token for user 'user_456' at the 'advanced-verification' level."

**🤖 AI Agent:**
> Generated token: 'sb:eyJhbG...'. You can use this token to initialize the Sumsub WebSDK for 'user_456'.


## ❓ FAQ

**Q: Can I check if a specific user has passed their KYC verification?**
Yes. Use the `get_applicant_status` tool with the Applicant ID. The AI will return the current verification stage and whether they are approved, pending, or rejected.

**Q: How do I provide a verification link to my users?**
You can use the `generate_access_token` tool. It provides the necessary token to initialize the Sumsub WebSDK for a specific User ID and verification level.

**Q: Is it possible to upload a user's ID document directly through the agent?**
Yes, by using the `add_document` tool. You will need the Applicant ID, the document type (like PASSPORT), the country code, and the base64 encoded content of the file.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sumsub](https://vinkius.com/mcp/sumsub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sumsub** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `sumsub` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sumsub** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sumsub": {
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
