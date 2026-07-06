# Hunter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hunter-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Find and verify professional email addresses with domain search, email finder, and deliverability verification for sales outreach.

## Description
Connect your **Hunter** account to any AI agent and power your email prospecting through natural conversation.

### What you can do

- **Domain Search** — Find all professional email addresses associated with a domain or company name
- **Email Finder** — Discover the most likely email address for a specific person by name and company
- **Email Verification** — Check the validity and deliverability of any email address with confidence scores
- **Email Count** — Check how many email addresses are available for a domain before searching
- **Contact Enrichment** — Retrieve all available professional data (title, company, social profiles) for an email address
- **Lead Management** — Create, list, update, and delete leads in your Hunter CRM with lead list organization
- **Account Monitoring** — Track remaining API credits and account usage

### How it works

1. Subscribe to this server
2. Enter your Hunter API Key from the account dashboard
3. Start finding emails from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Teams** — find decision-maker emails, verify addresses before outreach, and save leads to your CRM
- **Recruiters** — discover candidate contact information by name and company
- **Marketing Teams** — build verified email lists, enrich contact databases, and manage prospecting pipelines


## Available Tools (12)
- **search_domain_emails**: Find emails for domain
- **get_domain_email_count**: Check email availability
- **find_person_email**: Find personal email
- **verify_email_address**: Check deliverability
- **get_account_usage**: Check credits
- **enrich_email_data**: Get contact intel
- **get_lead_details**: Get lead info
- **list_lead_folders**: List lead lists
- **list_saved_leads**: List lead profiles
- **update_lead_info**: Modify lead data
- **create_new_lead**: Save lead to CRM
- **remove_lead**: Delete lead record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hunter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all emails at stripe.com and verify the CTO's email address."

**🤖 AI Agent:**
> Domain search for 'stripe.com': 48 emails available. Top results: 1) patrick@stripe.com — Patrick Collison (CEO, confidence: 95%). Sources: 4 public web pages. 2) john@stripe.com — John Collison (President, confidence: 92%). 3) david@stripe.com — David Singleton (CTO, confidence: 88%). 4) claire@stripe.com — Claire Hughes Johnson (COO, confidence: 85%). Verifying CTO email: david@stripe.com — ✅ Status: deliverable. Confidence: 92%. MX records: valid (Google Workspace). SMTP check: passed. Accept-all: no. This email is safe for outreach. Would you like to save these as leads or enrich the contacts?

---

**👤 You:**
> "Find the email for Sarah Chen at Acme Corp and enrich her contact data."

**🤖 AI Agent:**
> Email found! sarah.chen@acmecorp.com — Confidence: 91%. Pattern used: {first}.{last}@acmecorp.com. Enrichment data: Full name: Sarah Chen. Title: VP of Engineering. Company: Acme Corp (acmecorp.com). Industry: SaaS. Employees: 250-500. LinkedIn: linkedin.com/in/sarahchen. Twitter: @sarahchen_tech. Location: San Francisco, CA. Previous: Senior Engineer at Google (2018-2022). Lead saved! ID: lead_4521. Added to 'Enterprise Prospects' list. Would you like to verify her email or search for more contacts at Acme Corp?

---

**👤 You:**
> "Check my Hunter account credits and list all saved leads."

**🤖 AI Agent:**
> Account: john@company.com. Plan: Starter. Credits this month: Searches: 18 of 500 used (482 remaining). Verifications: 42 of 1,000 used (958 remaining). Resets: May 1, 2025. Saved leads: 34 total. Lead lists: 1) 'Enterprise Prospects' — 12 leads (8 verified, 4 unverified). 2) 'SMB Outreach' — 15 leads (12 verified, 3 risky). 3) 'Recruiting Pipeline' — 7 leads (all verified). Recent leads: sarah.chen@acmecorp.com (VP Engineering, added today). david@stripe.com (CTO, added today). mike@techco.com (Director Sales, added yesterday). Would you like to verify unverified leads or search a new domain?


## ❓ FAQ

**Q: Can I find all professional email addresses for a specific company?**
Yes. Use `search_domain_emails` with a domain (e.g., 'stripe.com') or company name (e.g., 'Stripe') to retrieve all professional emails found for that organization. Each result includes the email, confidence score, position, and source URLs. Use `get_domain_email_count` to preview how many emails are available before using search credits.

**Q: Can I verify if an email address is valid before sending outreach?**
Yes. The `verify_email_address` tool checks the validity and deliverability of any email address. It returns a status (deliverable, undeliverable, risky, unknown), confidence score, and details about the email server (MX records, SMTP check, accept-all detection). This prevents bounces and protects your sender reputation.

**Q: How does Hunter API authentication work?**
Hunter uses an API Key passed as a query parameter (`?api_key=YOUR_KEY`) in all requests to `api.hunter.io/v2`. This differs from the typical Bearer token pattern. Your API key is available in the Hunter dashboard under Account > API. Free accounts include 25 searches and 50 verifications per month.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hunter-alternative](https://vinkius.com/mcp/hunter-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hunter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hunter-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hunter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hunter-alternative": {
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
