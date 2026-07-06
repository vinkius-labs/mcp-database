# Dalil AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dalil-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Build AI assistants that understand Arabic natively and serve Middle Eastern markets with culturally aware conversational AI.

## Description
Connect your **Dalil AI** account to any AI agent to streamline your outbound sales and multichannel outreach through natural conversation. Dalil AI provides a powerful platform for discovering deep B2B intelligence, automating LinkedIn engagement, and tracking real-time buying signals across your lead pipeline.

### What you can do

- **Contact Orchestration** — List and create potential prospects programmatically, retrieving detailed professional backgrounds and contact metadata to coordinate outreach
- **LinkedIn Automation** — Trigger the delivery of personalized messages and connection requests programmatically to maintain high-fidelity professional engagement
- **Company Discovery** — Access and monitor your tracked organizations and retrieve detailed firmographic and industry intelligence directly through your agent
- **Signal Intelligence** — Retrieve real-time buying signals for your contacts to prioritize high-intent opportunities and coordinate perfectly timed follow-ups
- **Campaign Monitoring** — Access your complete directory of outreach campaigns and monitor sales performance metrics directly from your agent

### How it works

1. Subscribe to this server
2. Retrieve your **Secret API Key** from your Dalil AI dashboard settings (usedalil.ai)
3. Start enriching leads and automating your LinkedIn outreach from Claude, Cursor, or any MCP client

No more manual LinkedIn task management or missing high-intent buying signals. Your AI acts as your dedicated sales associate and outreach coordinator.

### Who is this for?

- **Sales Development (SDRs)** — build highly targeted outreach lists and automate LinkedIn tasks using natural language commands
- **Account Executives (AEs)** — monitor buying signals across key accounts to identify high-intent opportunities without leaving your workspace
- **Growth Marketers** — integrate real-time sales intelligence and automated outreach into custom growth workflows through simple AI queries


## Available Tools (6)
- **create_contact**: Pass data as a JSON string.

Create a new contact
- **list_campaigns**: List outreach campaigns
- **list_companies**: List all tracked companies
- **list_contacts**: List all Dalil contacts
- **send_linkedin_message**: Pass data in JSON.

Send a LinkedIn message via Dalil
- **get_contact_signals**: Get buying signals for a contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dalil AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active contacts in Dalil AI."

**🤖 AI Agent:**
> I've retrieved your contact list. You currently have 150 prospects, including 'Sarah Jenkins' (CTO at TechCorp) and 'Michael Ross'. Would you like me to check for any buying signals for them?

---

**👤 You:**
> "Send a LinkedIn message to contact '123' saying 'Hi Sarah, great launch!'."

**🤖 AI Agent:**
> LinkedIn message dispatched! I've delivered your personalized greeting to Sarah Jenkins. The job is marked as 'Delivered'. Shall I monitor her response for you?

---

**👤 You:**
> "Show me the buying signals for 'Michael Ross'."

**🤖 AI Agent:**
> Fetching signals... Michael Ross recently updated his title to 'VP of Infrastructure' and his company just announced a new funding round. These are high-intent signals. Shall I draft a follow-up?


## ❓ FAQ

**Q: How do I find my Dalil AI API Key?**
Log in to your account at [usedalil.ai](https://usedalil.ai/), navigate to **Settings** or **API**, and copy your unique secret key.

**Q: Can I automate LinkedIn messages with dynamic text?**
Yes! The `send_linkedin_message` tool allows your agent to dispatch personalized content directly to a contact's LinkedIn profile.

**Q: What kind of buying signals does Dalil provide?**
Dalil provides real-time indicators such as job changes, company funding rounds, and strategic shifts that signal high purchase intent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dalil-ai](https://vinkius.com/mcp/dalil-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dalil AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dalil-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dalil AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dalil-ai": {
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
