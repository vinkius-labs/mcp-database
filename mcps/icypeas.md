# Icypeas MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/icypeas)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Lead generation and email verification via Icypeas API.

## Description
Empower your AI agents to build and verify your lead database with Icypeas. This MCP server allows you to list prospects, search for specific leads, manage prospect lists, verify email deliverability, and find contact information directly through the Icypeas API. Ideal for automating sales outreach and lead enrichment.


## Available Tools (9)
- **count_people**: Uses same filter format as find_people.

Count the number of people matching a query (does not consume credits)
- **domain_scan**: Returns a search ID — use fetch_results to retrieve found emails.

Scan a domain for all role-based email addresses (contact@, admin@, etc)
- **fetch_results**: Pass the _id returned by those tools. If mode=single, lists all single searches. Max 100 results per request.

Retrieve results from previous searches by ID or list all single/bulk searches
- **find_companies**: Returns enriched company profiles.

Search the lead database for companies matching filters
- **find_email**: Returns a search ID — use fetch_results to get the actual email once status is DEBITED.

Find an email address for a person at a company domain
- **find_people**: Returns enriched profiles. Use JSON filter format: {"currentJobTitle": {"include": ["CTO"]}, "location": {"include": ["US"]}}

Search the lead database for people matching filters
- **get_subscription**: Get subscription information and remaining credits
- **reverse_email_lookup**: Find the profile URL behind a professional email address
- **verify_email**: Returns a search ID — use fetch_results to get verification status.

Verify the deliverability of an email address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Icypeas** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all prospects in my 'Tech Startup' list."

**🤖 AI Agent:**
> I'll retrieve the prospect list for 'Tech Startup' from Icypeas.

---

**👤 You:**
> "Verify if the email 'john@example.com' is deliverable."

**🤖 AI Agent:**
> I'll check the deliverability of that email address for you.

---

**👤 You:**
> "Find the email for Jane Doe at stripe.com."

**🤖 AI Agent:**
> I'll use Icypeas to find the contact information for that person.


## ❓ FAQ

**Q: How do I get Icypeas API credentials?**
You can find your API key in your Icypeas dashboard under 'Account Settings'.

**Q: Does email verification cost credits?**
Yes, using the verify_email and find_email tools will consume credits from your Icypeas account.

**Q: Can I see my remaining credits?**
Yes, the get_credits tool allows you to check your current credit balance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/icypeas](https://vinkius.com/mcp/icypeas)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Icypeas** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `icypeas` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Icypeas** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "icypeas": {
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
