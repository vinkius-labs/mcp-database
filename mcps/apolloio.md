# Apollo.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apolloio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Power your sales engagement with Apollo.io — search for prospects, enrich contact data, and manage sequences via AI.

## Description
The **Apollo.io MCP Server** provides direct access to one of the world's largest B2B databases. Connect your Apollo account to your AI agent to automate prospecting, data enrichment, and outreach workflows using natural language.

### What you can do

- **Targeted Prospecting** — Search for people and organizations using granular filters like job titles, industries, and locations.
- **Data Enrichment** — Instantly fill in missing details for people and companies. Get verified emails, phone numbers, and company insights.
- **Engagement Automation** — List your sales sequences and add new contacts to them directly from your chat.
- **Workspace Management** — Search and manage your saved contacts within your Apollo workspace.

### How it works

1. Subscribe to this server
2. Provide your Apollo API Key
3. Start discovering and engaging with leads through your AI chat interface.

### Who is this for?

- **Sales Development Representatives (SDRs)** — Rapidly build lead lists and trigger outreach sequences without manual data entry.
- **Marketing Teams** — Enrich existing customer data with company-level insights for better segmentation.
- **Recruiters** — Search the Apollo database for specific professional profiles and talent pools.


## Available Tools (8)
- **search_contacts**: Search Apollo contacts
- **search_organizations**: Search organizations
- **get_contact**: Get contact by ID
- **list_email_accounts**: List connected email accounts
- **list_sequences**: List sequences/campaigns
- **add_contact_to_sequence**: Add contact to sequence
- **get_call**: Get call details
- **search_people**: Search mixed people


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Apollo.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find people with the title 'CEO' in the 'Software' industry located in San Francisco."

**🤖 AI Agent:**
> I've found 25 profiles matching your criteria. Top results include the CEOs of several high-growth startups in San Francisco. Would you like me to enrich the first 5 to get their emails?

---

**👤 You:**
> "Enrich the organization data for 'vinkius.com'."

**🤖 AI Agent:**
> I've enriched the data for Vinkius. They are in the Computer Software industry, with approximately 50-100 employees, and are based in Brazil. They use technologies like React and Node.js.

---

**👤 You:**
> "Add contact 'c_123' to my 'New Year Campaign' sequence."

**🤖 AI Agent:**
> I've successfully added contact 'c_123' to the 'New Year Campaign' sequence (ID: seq_456). The first email will be sent according to your sequence schedule.


## ❓ FAQ

**Q: How do I get an Apollo API Key?**
Log in to your Apollo.io account, go to **Settings > Integrations > API**, and generate a new API key. Ensure you have the necessary permissions based on your plan.

**Q: Does searching for people consume credits?**
Basic searching typically does not consume credits, but 'enriching' a contact to reveal their verified email or phone number will consume Apollo export credits according to your subscription plan.

**Q: Can I add contacts directly to my sequences?**
Yes! Use the `add_contact_to_sequence` tool. You'll need the Contact IDs, the Sequence ID, and the ID of the email address you want to use for the outreach.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apolloio](https://vinkius.com/mcp/apolloio)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `apolloio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Apollo.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "apolloio": {
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
