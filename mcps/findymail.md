# Findymail MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/findymail)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Find and verify verified B2B emails and direct phone numbers using natural language agents.

## Description
Connect your **Findymail** account to any AI agent and supercharge your sales prospecting and data enrichment workflows through the power of the Model Context Protocol (MCP). Findymail is designed for high-growth sales teams that need accurate, verified contact data without the manual grind of searching through LinkedIn or guessing email patterns.

### What you can do

- **Precision Email Finding** — Instantly retrieve verified B2B emails by providing a person's name and their company domain or name. No more guessing; get data that actually delivers.
- **Real-time Email Verification** — Protect your sender reputation by verifying any email address before it hits your outreach sequence. Our verification tool checks for deliverability in seconds.
- **Direct Phone Discovery** — Scale your cold calling efforts by fetching direct phone numbers directly from LinkedIn profiles using our specialized phone finder tool.
- **Deep Company Enrichment** — Transform a simple domain or LinkedIn URL into a full company profile, including industry data, size, and social identifiers.
- **Intellimatch Lead Generation** — Use natural language to discover new leads. Simply ask your agent to 'Find SaaS founders in the US' or 'Get me marketing heads in London', and let Findymail do the heavy lifting.
- **List & Contact Management** — Organically manage your prospecting lists and retrieve specific contact details to keep your CRM updated and your outreach personalized.
- **Credit Monitoring** — Keep a pulse on your API usage with built-in tools to check your remaining credits and usage summaries directly from your AI conversation.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Findymail API Token (found in your dashboard settings)
3. Start managing your lead generation directly from Claude, Cursor, or any MCP-compatible environment

### Who is this for?

- **SDRs & BDRs** — find the right contacts for your target accounts without leaving your AI assistant, saving hours of manual data entry.
- **Marketing Operations** — ensure your lead lists are clean, verified, and enriched with the latest metadata before launching major campaigns.
- **Founders & Recruiters** — quickly identify and reach out to key decision-makers or potential candidates with verified direct contact information.


## Available Tools (12)
- **get_credits_summary**: Get credits usage summary
- **get_credits**: Check credit balance
- **get_lead_search_data**: Get lead search results
- **get_lead_search_status**: Check lead search status
- **list_contact_lists**: List all contact lists
- **search_leads**: Find companies and contacts
- **verify_email**: Verify an email address
- **create_contact_list**: Create a new contact list
- **enrich_company**: Enrich company data
- **find_email**: Find a verified email address
- **find_phone**: Find direct phone numbers
- **get_contact**: Get contact details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Findymail** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the verified email for Satya Nadella at microsoft.com"

**🤖 AI Agent:**
> Searching... I found a verified email for Satya Nadella at Microsoft. The email is verified and safe to send.

---

**👤 You:**
> "Enrich company data for the domain 'vinkius.com'"

**🤖 AI Agent:**
> Fetching data... I've retrieved the company profile for Vinkius, including LinkedIn URL, industry, and size metrics.

---

**👤 You:**
> "Search for 'marketing agency owners in New York' using Intellimatch."

**🤖 AI Agent:**
> Lead search task started! The Task ID is 'task_123'. I will check the status and notify you when the results are ready to be fetched.


## ❓ FAQ

**Q: How does Findymail ensure the accuracy of the found emails?**
Findymail uses a proprietary verification engine that checks the deliverability of B2B emails in real-time. By using the 'verify_email' tool, you can double-check any address to ensure your bounce rate stays below 1%.

**Q: Can I search for leads using natural language like 'Founders in San Francisco'?**
Yes! The 'search_leads' tool uses the Intellimatch engine, allowing you to discover companies and contacts based on conversational queries. It's like having a lead researcher built into your AI agent.

**Q: What happens if a phone number or email cannot be found?**
If Findymail cannot locate a verified contact, the tool will return a null or empty status. Findymail only charges credits for successful finds, ensuring you only pay for data you can actually use.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/findymail](https://vinkius.com/mcp/findymail)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Findymail** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `findymail` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Findymail** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "findymail": {
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
