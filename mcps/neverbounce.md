# NeverBounce MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/neverbounce)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Verify and clean email addresses via NeverBounce — track single checks and bulk jobs directly from your AI agent.

## Description
Connect your **NeverBounce** account to your AI agent and ensure your email lists are clean and deliverable through natural conversation.

### What you can do

- **Real-time Verification** — Check a single email address instantly to get its status (valid, invalid, disposable, etc.).
- **Bulk Job Management** — Create, parse, and start bulk verification jobs from URLs or raw input arrays.
- **Progress Tracking** — Monitor the status and progress of your active bulk jobs in real-time.
- **Result Retrieval** — Fetch the verification results for all emails in a completed job for download or analysis.
- **Account Oversight** — Check your remaining credit balance and list all recent jobs in your history.
- **Deep Inspection** — Fetch detailed metadata and flags for specific email checks or job IDs.

### How it works

1. Subscribe to this server
2. Enter your NeverBounce API Key
3. Start cleaning your email lists from Claude, Cursor, or any MCP client

### Who is this for?

- **Marketing Teams** — quickly verify a lead's email before adding it to a campaign.
- **Sales Operations** — automate the cleaning of prospect lists directly from your chat tool.
- **Developers** — integrate real-time email verification into your workflows through natural language commands.


## Available Tools
- **check_email**: Verify a single email address
- **create_job_from_input**: Create a bulk job from raw input
- **create_job_from_url**: Create a bulk job from a remote CSV URL
- **delete_job**: Delete a bulk job
- **get_account_info**: Get account credits and info
- **get_job_results**: Get results of a completed bulk job
- **get_job_status**: Check status of a bulk job
- **list_jobs**: List bulk verification jobs
- **parse_job**: Parse a bulk job
- **start_job**: Start a bulk job


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NeverBounce** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Verify if the email 'test@example.com' is valid."

**🤖 AI Agent:**
> Checking email... The result for 'test@example.com' is VALID. No deliverability issues were found and no flags were raised. Shall I check your remaining credits?

---

**👤 You:**
> "List all my recent verification jobs."

**🤖 AI Agent:**
> Retrieving your jobs... I found 3 recent jobs: 'Lead List Q1' (Status: Completed), 'Prospects March' (Status: Running), and 'Web Signups' (Status: Parsing). Would you like the results for 'Lead List Q1'?

---

**👤 You:**
> "Check the status of job ID 123456."

**🤖 AI Agent:**
> Inspecting job 123456... This job is currently 75% complete. Out of 1,000 emails, 600 have been verified as Valid and 150 as Invalid so far. I'll let you know when it reaches 100%.


## ❓ FAQ

**Q: Where do I find my NeverBounce API Key?**
Log in to your NeverBounce dashboard and navigate to the API section to create or copy your 'Secret Key'.

**Q: What do the different result statuses mean?**
'Valid' means the email is safe to send. 'Invalid' will bounce. 'Disposable' are temporary addresses, and 'Catchall' means the domain accepts all mail, making deliverability uncertain.

**Q: How do I start a bulk verification job?**
First, use `create_job_from_url` or `create_job_from_input`. Then, call `parse_job` followed by `start_job` to begin the verification process.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/neverbounce](https://vinkius.com/mcp/neverbounce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NeverBounce** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `neverbounce` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NeverBounce** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "neverbounce": {
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
