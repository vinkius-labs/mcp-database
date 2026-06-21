# FindThatLead MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/findthatlead)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Uncover business email addresses from domain names and LinkedIn profiles to fuel your outbound prospecting pipeline.

## Description
Connect your **FindThatLead** account to any AI agent and take full control of your B2B lead discovery and email verification workflows through natural conversation.

### What you can do

- **Domain Intelligence** — Find all email addresses associated with any company domain programmatically and retrieve detailed contact metadata
- **Email Discovery** — Locate specific professional email addresses using a person's first name, last name, and company domain directly through your agent
- **High-Fidelity Verification** — Programmatically verify the validity and deliverability of any email address using a multi-step verification algorithm
- **Prospecting Automation** — Perform local business searches by keyword and location to discover new leads and automate your outreach pipeline
- **Campaign Monitoring** — Access your saved lead lists and outreach campaigns programmatically to monitor engagement and acquisition progress

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from the FindThatLead dashboard (Settings > API Access)
3. Start generating and verifying B2B leads from Claude, Cursor, or any MCP client

No more manual copy-pasting into email verifiers or complex domain searching. Your AI acts as your dedicated sales development and lead generation assistant.

### Who is this for?

- **Sales SDRs & BDRs** — instantly find contact details for target prospects and verify deliverability using natural language
- **Growth Marketers** — automate the extraction of leads from specific company domains and locations without leaving your workspace
- **Recruiters** — quickly locate professional email addresses for candidates through simple AI queries


## Available Tools
- **create_lead**: Save a new lead
- **delete_lead**: Remove a lead
- **domain_search**: Find emails for a domain
- **email_finder**: Find email for a specific person
- **email_verifier**: Verify an email address
- **get_account_info**: Get account details
- **get_campaign**: Get campaign details
- **get_lead**: Get lead details
- **get_account_stats**: Get account usage stats
- **list_campaigns**: List email campaigns
- **list_leads**: List saved leads
- **local_prospector**: Find local business leads


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FindThatLead** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all emails for the domain 'stripe.com'."

**🤖 AI Agent:**
> Scanning stripe.com... I've found 15 professional email addresses associated with this domain. Notable contacts include roles in 'Engineering' and 'Sales'. Would you like the full list of verified addresses?

---

**👤 You:**
> "Verify if 'test@example.com' is a valid email."

**🤖 AI Agent:**
> Verification complete! The email 'test@example.com' is marked as 'Invalid'. It failed the SMTP check and appears to be a non-deliverable address. Shall I help you find an alternative contact?

---

**👤 You:**
> "Find the email for 'John Doe' at 'acme.com'."

**🤖 AI Agent:**
> Locating John Doe... I've successfully found their professional email at acme.com. It is 'john.doe@acme.com' with a 95% confidence score. Would you like me to save this lead to your account?


## ❓ FAQ

**Q: How do I find my FindThatLead API Key?**
Log in to your FindThatLead account, navigate to **Settings** > **API Access**, and copy your unique token.

**Q: Does email verification consume credits?**
Yes, each successful email verification or lead search typically consumes one credit from your FindThatLead account balance.

**Q: Can I search for local businesses by city?**
Absolutely. Use the `local_prospector` tool and provide a keyword (e.g., 'Dentist') and a location to find businesses in that area.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/findthatlead](https://vinkius.com/mcp/findthatlead)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FindThatLead** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `findthatlead` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FindThatLead** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "findthatlead": {
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
