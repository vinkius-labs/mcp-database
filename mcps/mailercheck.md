# MailerCheck MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mailercheck)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Verify and validate email addresses in real-time or batch via the MailerCheck REST API.

## Description
Connect your **MailerCheck** account to any AI agent to automate your email hygiene and deliverability workflows. This MCP server enables your agent to verify single email addresses instantly, manage batch verification lists, and monitor your account credits directly from natural language interfaces.

### What you can do

- **Real-time Verification** — Instantly check if an email address is valid, risky, or invalid before sending
- **Batch Processing** — Upload large lists of emails for asynchronous validation and track their progress
- **Results Ingestion** — Retrieve detailed status reports for completed batches, including reason codes for invalid emails
- **History Oversight** — List all recent verification batches and retrieve their technical metadata
- **Account Auditing** — Monitor your authenticated user details and remaining verification credits

### How it works

1. Subscribe to this server
2. Enter your MailerCheck API Token
3. Start validating your email lists from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Email Marketers** — Maintain high sender reputation by cleaning contact lists via simple natural language commands
- **Sales & Outreach Teams** — Instantly verify lead emails before reaching out to minimize bounce rates
- **Growth Engineers** — Integrate email validation logic and batch monitoring directly into your development tools


## Available Tools (5)
- **get_account_info**: Get account details and credit balance
- **get_batch_results**: Retrieve the results for a specific batch
- **list_verification_batches**: List all recent verification batches
- **create_verification_batch**: Requires a name and a list of emails.

Upload a list of emails for batch verification
- **verify_single_email**: Requires an email string.

Verify a single email address in real-time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MailerCheck** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Verify the email address 'user@example.com' in MailerCheck."

**🤖 AI Agent:**
> I've checked the address. 'user@example.com' is marked as 🟢 VALID. You can safely send to this recipient.

---

**👤 You:**
> "List all my recent verification batches."

**🤖 AI Agent:**
> I've retrieved your batches. You have 3 recent jobs: 'Main Website Leads (ID: 123)', 'Old CRM Export', and 'Newsletter Cleanup'. Would you like to see the results for any of them?

---

**👤 You:**
> "Show valid emails for batch ID '123'."

**🤖 AI Agent:**
> I've queried the results for batch 123. There are 45 valid email addresses, including 'admin@corp.com' and 'sales@firm.io'. I've filtered out risky and invalid results.


## ❓ FAQ

**Q: What is the accuracy of MailerCheck verification?**
MailerCheck uses advanced multi-layer checks including syntax, DNS, and SMTP handshake to provide highly accurate results categorized into valid, risky, and invalid.

**Q: Can I verify large lists of emails?**
Yes, use the `create_verification_batch` tool to upload a JSON array of email addresses. You can then monitor the progress and retrieve results once completed.

**Q: How do I check my remaining credits?**
Use the `get_account_info` tool to retrieve your profile details and the current balance of verification credits in your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailercheck](https://vinkius.com/mcp/mailercheck)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MailerCheck** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mailercheck` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MailerCheck** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mailercheck": {
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
