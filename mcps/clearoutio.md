# Clearout.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clearoutio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Verify email addresses and deliverability via Clearout — track validation jobs, monitor credit balance, and audit list health directly from any AI agent.

## Description
Connect your **Clearout.io** account to any AI agent and take full control of your email verification and deliverability workflows through natural conversation. Streamline how you maintain list hygiene and protect your sender reputation natively.

### What you can do

- **Instant Verification** — Verify single email addresses in real-time to identify valid, invalid, or catch-all accounts natively
- **Bulk Intelligence** — Submit and monitor large email lists for asynchronous verification flawlessly
- **Deliverability Auditing** — Specifically check for disposable, catch-all, or role-based email addresses securely
- **Business Logistics** — Identify business vs. free/personal email accounts to target professional audiences flawlessly
- **Job Oversight** — List and retrieve the status of all current and historical bulk verification jobs flawlessly
- **Credit Tracking** — Retrieve your remaining verification credit balance directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Clearout API Token (obtained from Developer settings)
3. Start verifying your email lists from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Email Marketers** — monitor list hygiene and verify subscriber data using natural language
- **Sales Development** — audit lead lists and verify business emails without opening the dashboard
- **Product Teams** — quickly verify signup emails and monitor verification throughput straight from their chat interface
- **Marketing Ops** — verify credit usage and monitor bulk job progress


## Available Tools
- **get_bulk_verification_status**: Get the progress status of a bulk verification job
- **get_clearout_credit_balance**: Retrieve the remaining email verification credit balance
- **list_bulk_verification_jobs**: List all bulk verification jobs in the account
- **submit_bulk_email_list**: Submit a list of emails for bulk verification
- **check_business_email**: Check if an email belongs to a business or professional domain
- **check_email_catchall**: Specifically check if an email domain is configured as catch-all
- **check_disposable_email**: Check if an email address belongs to a disposable/temporary provider
- **verify_email_instant**: Verify a single email address in real-time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clearout.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Verify this email address: support@example.com"

**🤖 AI Agent:**
> Verifying support@example.com... The email is 'Valid'. It's a role-based business account at a professional domain.

---

**👤 You:**
> "What is my current credit balance in Clearout?"

**🤖 AI Agent:**
> Checking your credit balance... You currently have 12,450 credits remaining. Based on your current usage, this should cover approximately 25 more bulk cleanings.

---

**👤 You:**
> "Check if 'johndoe@gmail.com' is a business or personal email."

**🤖 AI Agent:**
> Analyzing email domain... 'johndoe@gmail.com' is classified as a 'Personal' email account using a free public provider.


## ❓ FAQ

**Q: Can I verify if an email is a temporary or disposable address?**
Yes! Use the `check_disposable_email` tool. The agent will check the email against Clearout's database of known disposable email providers and return a true/false result.

**Q: How do I check the progress of a large email list I uploaded?**
Use the `get_bulk_verification_status` tool with your list ID. Your agent will return the percentage completed, allowing you to monitor the cleaning process in real-time.

**Q: Where do I find my Clearout API Token?**
Log in to your Clearout dashboard, navigate to the **Developer** section, and select **API**. You can create and copy your API token from that page.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clearoutio](https://vinkius.com/mcp/clearoutio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Clearout.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `clearoutio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Clearout.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clearoutio": {
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
