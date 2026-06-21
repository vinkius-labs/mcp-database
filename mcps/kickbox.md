# Kickbox MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kickbox)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Verify email addresses in real-time or in bulk to improve deliverability and protect your sender reputation.

## Description
Connect **Kickbox** to your AI agent to ensure your email lists are clean, deliverable, and free of risky addresses. This server allows you to validate individual emails or process large batches directly through natural language.

### What you can do

- **Real-time Verification** — Instantly check if an email is deliverable, undeliverable, or risky before sending.
- **Batch Processing** — Start large-scale verification jobs for entire lists of email addresses.
- **Status Monitoring** — Track the progress of your batch jobs and retrieve results once completed.
- **Reputation Protection** — Identify disposable, role-based, or invalid emails to maintain a high sender score.

### How it works

1. Subscribe to this server
2. Enter your Kickbox API Key
3. Start verifying emails from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Teams** — Clean lead lists before launching campaigns to reduce bounce rates.
- **Developers** — Integrate email validation into registration flows or internal tools.
- **Sales Operations** — Ensure CRM data is accurate and outreach reaches the intended inbox.


## Available Tools
- **get_batch_status**: Check the status of a batch verification job
- **start_batch_verification**: Returns a Job ID to check status later.

Start a batch email verification job
- **verify_email**: Verify a single email address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kickbox** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Verify if the email 'test@example.com' is deliverable."

**🤖 AI Agent:**
> I've checked the email. The status for 'test@example.com' is 'deliverable'. It is safe to send to this address.

---

**👤 You:**
> "Start a batch verification for these emails: ['user1@gmail.com', 'user2@outlook.com', 'invalid-email@test']."

**🤖 AI Agent:**
> The batch verification job has been started. Your Job ID is 123456. You can check its progress using the get_batch_status tool.

---

**👤 You:**
> "What is the status of my Kickbox batch job 123456?"

**🤖 AI Agent:**
> The job 123456 is currently 'completed'. 100% of the emails have been processed. You can download the full report here: [Download URL].


## ❓ FAQ

**Q: Can I check if a single email address is valid before adding it to my database?**
Yes! Use the `verify_email` tool with the email address. The agent will return real-time results indicating if the email is deliverable, undeliverable, or risky.

**Q: How do I verify a large list of emails at once?**
You can use the `start_batch_verification` tool. Provide an array of email addresses, and the server will start a background job and return a Job ID for tracking.

**Q: How can I check if my batch verification job is finished?**
Use the `get_batch_status` tool with your Job ID. It will provide the current status (processing, completed, etc.), progress percentage, and a download URL if the job is done.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kickbox](https://vinkius.com/mcp/kickbox)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kickbox** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `kickbox` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kickbox** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kickbox": {
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
