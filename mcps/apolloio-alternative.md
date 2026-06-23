# Apollo.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apolloio-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Prospect smarter with verified contact data, enrich leads in real time, and build targeted sales sequences that convert.

## Description
Connect your **Apollo.io** account to any AI agent and take full control of your B2B prospecting and sales engagement workflows through natural conversation.

### What you can do

- **Prospect Orchestration** — Search through a massive database of professionals by title, location, and company domains programmatically in real-time
- **Data Enrichment Intelligence** — Programmatically retrieve verified email addresses, phone numbers, and high-fidelity social metadata for any contact or company
- **Sequence Lifecycle Management** — Enroll qualified leads into automated email sequences and monitor your sales outreach pipeline directly through your agent
- **Company Architecture** — Access deep firmographic data, including revenue, headcount, and technology stacks to maintain a perfectly coordinated account strategy
- **Operational Monitoring** — Track your remaining search and enrichment credits and monitor API connectivity directly through your agent for instant reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Apollo dashboard (Settings > Integrations > API)
3. Start orchestrating your sales pipeline from Claude, Cursor, or any MCP client

No more manual toggling between browser tabs to find emails or check prospect status. Your AI acts as your dedicated sales analyst and outreach coordinator.

### Who is this for?

- **Sales Development (SDRs)** — instantly build highly targeted prospect lists using natural language commands
- **Account Executives (AEs)** — enrich key account metadata and monitor buying intent without leaving your creative workspace
- **Growth Marketers** — automate lead enrichment and sequence enrollment through simple AI queries


## Available Tools (12)
- **add_to_sequence**: Enroll contact in sequence
- **enrich_company_data**: Get company metadata
- **enrich_person_data**: Get full profile details
- **get_saved_contact**: Get contact by ID
- **get_credit_info**: Get usage and credits
- **list_connected_emails**: Get sender accounts
- **get_api_health**: Get API and account status
- **list_sales_sequences**: List email sequences
- **list_team_users**: List account users
- **search_companies**: Find organizations
- **search_people**: Find prospects
- **list_saved_contacts**: List your contacts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Apollo.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the 'VP of Engineering' at 'vinkius.com'."

**🤖 AI Agent:**
> I've performed the high-fidelity search. I found the 'VP of Engineering' at Vinkius (ID: person_123) with a verified email. Would you like me to enrich their profile for LinkedIn and phone details?

---

**👤 You:**
> "Show the tech stack and revenue for 'apple.com'."

**🤖 AI Agent:**
> Accessing company intelligence... Apple Inc. (Domain: apple.com) has an estimated revenue of $380B+ and uses 150+ technologies including AWS, Akamai, and React. Need the high-fidelity detailed list of employees?

---

**👤 You:**
> "Enroll contact '123' into sales sequence '456'."

**🤖 AI Agent:**
> Enrollment complete! I've successfully added contact 123 to sequence 456. The automated outreach will begin according to your schedule. Shall I alert you when the first email is opened?


## ❓ FAQ

**Q: How do I find my Apollo API Key?**
Log in to your account, navigate to **Settings** > **Integrations** > **API**, and generate or copy your unique personal token.

**Q: Can I enrich a company by its domain via AI?**
Yes! The `enrich_company_data` tool allows your agent to retrieve high-fidelity metadata like revenue and tech stack using just the company domain.

**Q: How do I check my remaining credits?**
Use the `get_credit_info` tool to retrieve real-time data on your search and enrichment quotas directly through your AI agent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apolloio-alternative](https://vinkius.com/mcp/apolloio-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Apollo.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `apolloio-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Apollo.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "apolloio-alternative": {
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
