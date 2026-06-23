# Cleared (ClearedIn) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cleared-clearedin)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Manage identity verification and background screening via Cleared — track verifications, monitor screenings, and audit security logs directly from any AI agent.

## Description
Connect your **Cleared (ClearedIn)** account to any AI agent and take full control of your identity verification and screening workflows through natural conversation. Streamline how you verify users and maintain trust natively.

### What you can do

- **Verification Oversight** — List and retrieve details for all identity verification requests and their status natively
- **Screening Intelligence** — Access and monitor background screening requests and retrieve detailed results flawlessly
- **Digital Signatures** — List all digital signature requests and track their completion status securely
- **Audit Logistics** — Access security audit logs to track who accessed sensitive data and when flawlessly
- **Identity Management** — Retrieve core account and user metadata directly within your workspace flawlessly
- **Trust Logistics** — Monitor the lifecycle of verification sessions from 'Pending' to 'Verified' or 'Rejected' in real-time

### How it works

1. Subscribe to this server
2. Enter your Cleared API Key (obtained from the Admin Portal)
3. Start managing your identity verifications from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Compliance Officers** — monitor identity verification volumes and status using natural language
- **HR Managers** — audit background screening results without opening the admin portal
- **Security Teams** — quickly look up audit logs and verification details straight from their chat interface
- **Operations Teams** — verify signature completion and session health


## Available Tools (8)
- **get_cleared_account_info**: Retrieve core account and user metadata
- **get_screening_details**: Get detailed results for a specific screening
- **get_signature_details**: Get detailed status for a specific signature request
- **get_verification_details**: Get detailed information for a specific verification
- **list_cleared_audit_logs**: List security audit logs for the account
- **list_background_screenings**: List all background screening requests
- **list_digital_signatures**: List all digital signature requests
- **list_identity_verifications**: List all identity verification requests


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cleared (ClearedIn)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 identity verifications in Cleared."

**🤖 AI Agent:**
> Retrieving your recent verifications... I found 5 items: John Doe (Verified), Jane Smith (Pending), Mike Scott (Rejected), and 2 others. Would you like the details for the pending request?

---

**👤 You:**
> "Show me the results for screening ID 'scr_12345'."

**🤖 AI Agent:**
> Checking screening scr_12345... This background check for 'Jane Doe' has been completed. Status: Cleared. All requested checks (Criminal, Employment, Education) were successful.

---

**👤 You:**
> "What is the status of the signature request for 'Employment Contract'?"

**🤖 AI Agent:**
> Retrieving signature status... The 'Employment Contract' sent to John Doe is currently 'Partially Signed'. The employer has signed, but the candidate is still pending.


## ❓ FAQ

**Q: Can I see if a user has finished their background check?**
Yes! Use the `get_screening_details` tool with the screening ID. The agent will return the current status and the final result of the check.

**Q: How do I find out who accessed a specific verification record?**
Use the `list_cleared_audit_logs` tool. Your agent will fetch the account's security logs, allowing you to audit access to sensitive personal information.

**Q: Where do I find my Cleared API Key?**
Log in to your Cleared (ClearedIn) Admin Portal and navigate to the **Integrations** section. You can generate and copy your API key from there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cleared-clearedin](https://vinkius.com/mcp/cleared-clearedin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cleared (ClearedIn)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cleared-clearedin` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cleared (ClearedIn)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cleared-clearedin": {
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
