# Clearout MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clearout)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Verify email addresses in bulk before sending campaigns to protect your sender reputation and improve deliverability rates.

## Description
Connect your **Clearout** email intelligence account to any AI agent and simplify how you clean your contact lists, verify deliverability, and discover professional email addresses through natural conversation.

### What you can do

- **Email Verification** — Instantly check if an email address is valid, active, and safe for your outreach campaigns.
- **Lead Discovery** — Find professional email addresses for prospects using only their full name and company domain.
- **Deliverability Protection** — Identify disposable, role-based, or catch-all addresses to protect your sender reputation.
- **Credit Monitoring** — Track your account usage and remaining API credits directly from the agent.
- **Real-time Validation** — Integrate verification into your automated workflows via simple AI commands.
- **Prospect Insights** — Verify lead data quality before adding them to your CRM or marketing machine.

### How it works

1. Subscribe to this server
2. Enter your Clearout API Key (found in your account dashboard under API)
3. Start validating your audience from Claude, Cursor, or any MCP client

### Who is this for?

- **Sales & SDR Teams** — quickly find prospect emails and verify lead lists via simple AI commands.
- **Marketing Managers** — clean campaign lists and monitor sender reputation directly from the workspace.
- **Growth Engineers** — automate email validation and verify credit balances via the AI assistant.


## Available Tools
- **cancel_bulk**: Already processed emails retain their results.

Cancel a bulk verification
- **check_clearout_status**: Verify Clearout API connectivity
- **download_results**: Download verification results
- **find_email**: Find a business email
- **get_bulk_status**: Check bulk verification progress
- **get_credits**: Check credit balance
- **remove_bulk_list**: Remove a bulk list
- **verify_bulk**: Returns a list ID to track progress.

Verify emails in bulk
- **verify_catchall**: Verify catch-all domain
- **verify_email**: Verify a single email


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clearout** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Verify if the email 'john.doe@example.com' is safe to send to."

**🤖 AI Agent:**
> Verification complete! The email 'john.doe@example.com' is marked as 'Valid' with a deliverability score of 98/100. It is a legitimate corporate address and safe for your campaign.

---

**👤 You:**
> "Find the professional email for 'Steve Jobs' at 'apple.com'."

**🤖 AI Agent:**
> I've attempted to find the address. Clearout suggests 'steve@apple.com' with a high confidence score. Would you like me to verify its deliverability as well?

---

**👤 You:**
> "How many validation credits do I have left?"

**🤖 AI Agent:**
> Checking credits... You currently have 4,520 validation credits remaining in your Clearout account. This is sufficient for your upcoming bulk list cleaning.


## ❓ FAQ

**Q: Can I verify if an email address is valid via AI?**
Yes! Use the `verify_email_address` tool and provide the address. Your agent will return its status (Valid, Invalid, etc.) and deliverability score.

**Q: How do I find a person's professional email using the agent?**
Use the `find_prospect_email` tool. Provide the person's full name and their company domain (e.g., 'example.com'). Clearout will attempt to locate the verified address.

**Q: Is it possible to check my remaining API credits via AI?**
Absolutely. Use the `check_api_credits` query. The agent will retrieve your current account balance, helping you monitor your validation budget.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clearout](https://vinkius.com/mcp/clearout)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Clearout** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `clearout` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Clearout** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clearout": {
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
