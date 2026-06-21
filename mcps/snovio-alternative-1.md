# Snov.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/snovio-alternative-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Find, verify, and manage leads with Snov.io — search domain emails, verify addresses, and add prospects to lists directly from your AI agent.

## Description
Connect your **Snov.io** account to any AI agent to automate your lead generation and sales outreach workflows through natural conversation.

### What you can do

- **Domain Search** — Find email addresses associated with any company domain name to identify key decision-makers.
- **Email Verification** — Check the validity of email addresses to reduce bounce rates and protect your sender reputation.
- **Prospect Management** — Add new leads directly to your Snov.io lists with names and contact details for immediate campaign inclusion.

### How it works

1. Subscribe to this server
2. Enter your Snov.io API Credentials (Client ID and Client Secret)
3. Start finding and verifying leads from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Development Reps (SDRs)** — quickly find contact info for target accounts without leaving the chat interface.
- **Marketing Teams** — verify large lists of emails to ensure high deliverability for outreach campaigns.
- **Recruiters** — identify and save potential candidates' contact details directly into organized lists.


## Available Tools (3)
- **add_prospect**: io account.

Add a prospect to a Snov.io list
- **domain_search**: io database for email addresses belonging to a company domain name.

Find email addresses associated with a specific domain
- **verify_emails**: Check the validity of email addresses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Snov.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find personal email addresses for the domain 'stripe.com' with a limit of 10 results."

**🤖 AI Agent:**
> I've searched Snov.io for stripe.com. I found 10 personal email addresses including 'john.doe@stripe.com' and 'jane.smith@stripe.com'. Would you like to verify any of these?

---

**👤 You:**
> "Verify the following emails: contact@example.com, test@invalid.com."

**🤖 AI Agent:**
> Verification complete: 'contact@example.com' is VALID, while 'test@invalid.com' is INVALID. I recommend removing the invalid address from your list.

---

**👤 You:**
> "Add 'Alice Johnson' (alice@company.com) to my Snov.io list with ID 987654."

**🤖 AI Agent:**
> Successfully added Alice Johnson to list 987654. She is now ready for your outreach campaigns.


## ❓ FAQ

**Q: How can I find all email addresses for a specific company domain?**
Use the `domain_search` tool by providing the target domain (e.g., 'example.com'). You can also filter by type (personal or generic) and set a limit on the number of results.

**Q: Can I verify if a list of emails is safe to send to?**
Yes! Use the `verify_emails` tool with an array of email addresses. The agent will return the verification status for each, identifying valid, invalid, or catch-all addresses.

**Q: How do I add a new lead to a specific Snov.io list?**
Use the `add_prospect` action. Provide the email address and the `listId`. You can also optionally include the prospect's first and last name.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/snovio-alternative-1](https://vinkius.com/mcp/snovio-alternative-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Snov.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `snovio-alternative-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Snov.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "snovio-alternative-1": {
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
