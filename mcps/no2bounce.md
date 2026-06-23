# No2Bounce MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/no2bounce)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Validate email addresses in bulk to reduce bounce rates and protect your sender reputation directly from your AI agent.

## Description
Connect **No2Bounce** to your AI agent to ensure your email lists are clean and deliverable. This server allows you to verify single or bulk email addresses, helping you maintain a high sender reputation and improve campaign performance without leaving your workflow.

### What you can do

- **Bulk Validation** — Submit lists of email addresses for real-time or asynchronous verification.
- **Status Tracking** — Monitor the progress of large validation tasks using unique tracking IDs.
- **Result Retrieval** — Fetch detailed validation results once processing is complete.
- **Spam Prevention** — Identify invalid, disposable, or high-risk email addresses before they hit your mailing list.

### How it works

1. Subscribe to this server
2. Enter your No2Bounce API Token
3. Start validating emails from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Email Marketers** — Clean lists before launching campaigns to ensure maximum deliverability.
- **Sales Teams** — Verify leads from scraped or purchased lists before outreach.
- **Developers** — Integrate email verification into registration or contact forms via AI-driven automation.


## Available Tools (2)
- **get_validation_status**: Check validation status or get final results
- **validate_bulk**: Returns a trackingId to check status later.

Submit a list of emails for validation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **No2Bounce** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate these emails for me: contact@company.com, support@service.io, invalid-email@test."

**🤖 AI Agent:**
> I've submitted 3 emails for validation. Your tracking ID is `nb_84729`. I'll check the status for you in a moment.

---

**👤 You:**
> "Check the status of my No2Bounce validation task nb_84729."

**🤖 AI Agent:**
> The validation for task `nb_84729` is complete. Results: 2 valid emails, 1 invalid. Would you like to see the detailed breakdown?

---

**👤 You:**
> "Submit this list of 10 emails to No2Bounce and give me the tracking ID."

**🤖 AI Agent:**
> Bulk validation started for 10 addresses. Your tracking ID is `nb_99210`. You can ask me to check the results using this ID later.


## ❓ FAQ

**Q: How do I submit multiple emails for validation at once?**
Use the `validate_bulk` tool and provide an array of email addresses in the `emailList` parameter. The server will return a `trackingId` which you can use to check the results.

**Q: How can I check if my bulk validation task is finished?**
You can use the `get_validation_status` tool by providing the `trackingId` received during the submission. It will return the current progress or the final validation results.

**Q: Is there a way to prevent sending the same validation request twice?**
Yes, when using `validate_bulk`, you can provide an optional `hashkey`. This unique string prevents duplicate requests from being processed within a 3-minute window.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/no2bounce](https://vinkius.com/mcp/no2bounce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **No2Bounce** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `no2bounce` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **No2Bounce** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "no2bounce": {
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
