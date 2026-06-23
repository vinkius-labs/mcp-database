# Hunter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hunter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Equip your AI agent with direct access to Hunter.io — find professional email addresses, verify deliverability, and enrich lead data without leaving your workflow.

## Description
Connect **Hunter.io** to your AI agent and power your lead generation with verified email discovery and enrichment.

### What you can do

- **Domain Search** — Find all professional email addresses associated with any company domain.
- **Email Finder** — Locate a specific person's email using their name and company domain.
- **Email Verification** — Verify if an email address is valid, deliverable, and safe to send to.
- **Lead Lists** — Create and manage lead lists with verified contacts for outreach campaigns.

### How it works

1. Subscribe to the Hunter integration on the marketplace.
2. Copy your API key from your Hunter.io dashboard (API section in the left sidebar).
3. Ask your AI agent to find emails, verify addresses, or search domains.

### Who is this for?

- **SDR Teams** — Find decision-maker emails instantly and verify them before adding to outreach sequences.
- **Growth Marketers** — Build targeted prospect lists by domain with verified, deliverable email addresses.
- **Recruiters** — Locate candidate email addresses by name and company for direct outreach.


## Available Tools (10)
- **domain_search**: Search emails by domain
- **list_recipients**: List campaign recipients
- **email_finder**: Find specific email
- **email_verifier**: Verify email address
- **email_count**: Count emails for domain
- **list_leads**: List saved leads
- **list_lead_lists**: List lead lists
- **get_account**: Get account info
- **list_campaigns**: List campaigns
- **get_campaign**: Get campaign details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hunter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all email addresses at stripe.com."

**🤖 AI Agent:**
> I found 47 email addresses at stripe.com. Most common pattern: {first}@stripe.com. Top results: john@stripe.com (CEO, confidence: 95%), sarah@stripe.com (VP Engineering, confidence: 91%), and 45 more.

---

**👤 You:**
> "Find the email for Sarah Johnson at Acme Corp."

**🤖 AI Agent:**
> Found: sarah.johnson@acmecorp.com (confidence: 92%). Email pattern at acmecorp.com: {first}.{last}. Verified status: valid. Position: VP Marketing. Sources: 3 public pages.

---

**👤 You:**
> "Verify if contact@oldstartup.io is still valid."

**🤖 AI Agent:**
> Verification result: INVALID. The MX records for oldstartup.io are not configured — the domain's email server is unreachable. Do not send to this address. I recommend removing it from your outreach list.


## ❓ FAQ

**Q: How do I get my Hunter.io API key?**
Log in to your Hunter.io account at **hunter.io**. In the left sidebar, click the **API** section (or go directly to **hunter.io/api-keys**). Your API key is displayed on this page. Click the **copy** button to copy it. Paste it into the configuration field below. Free plans include 25 searches and 50 verifications per month.

**Q: Can I find the email of a specific person at a company?**
Yes. Give your AI agent a person's first name, last name, and company domain, and it returns their most likely professional email address with a confidence score. Perfect for reaching out to specific decision-makers.

**Q: How accurate is the email verification?**
Hunter's verification checks MX records, SMTP responses, and catch-all configurations — returning a status of 'valid', 'invalid', 'accept_all', or 'unknown'. Valid emails have over 95% deliverability. Always verify before sending cold outreach to protect your sender reputation.

**Q: Does it work with free plans?**
Yes. Hunter offers a free plan with 25 email searches and 50 verifications per month. The API key works the same regardless of plan — the only difference is quota limits. Upgrade to a paid plan for higher volumes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hunter](https://vinkius.com/mcp/hunter)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `hunter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hunter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hunter": {
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
