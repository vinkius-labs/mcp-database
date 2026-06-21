# Amplemarket MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amplemarket-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Supercharge your outbound sales with AI-driven prospecting, multi-channel sequences, and smart lead scoring that closes deals.

## Description
Connect your **Amplemarket** account to any AI agent and take full control of your outbound sales engagement and high-fidelity lead enrichment workflows through natural conversation.

### What you can do

- **Lead & Company Enrichment** — Programmatically retrieve verified email addresses and deep firmographic data for any B2B contact or company domain in real-time
- **Outbound Sequence Intelligence** — Monitor the status and performance of your active sales sequences and retrieve high-fidelity campaign metrics directly through your agent
- **CRM Discovery** — Access complete directories of your saved sales contacts and retrieve granular profile metadata to coordinate your outreach strategy perfectly
- **Deliverability Oversight** — Access and monitor your exclusion lists and opt-out directories to maintain high-fidelity email health and sender reputation
- **Infrastructure Monitoring** — Verify API connectivity and retrieve account-level metadata directly through your agent for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Amplemarket dashboard (Settings > API)
3. Start orchestrating your outbound growth from Claude, Cursor, or any MCP client

No more manual toggling between sales tools or digging through complex CSV exports. Your AI acts as your dedicated sales analyst and outreach coordinator.

### Who is this for?

- **Sales Development (SDRs)** — instantly enrich prospect profiles and verify sequence statuses using natural language commands
- **Revenue Operations (RevOps)** — monitor global exclusion lists and campaign performance without leaving your creative workspace
- **Growth Marketers** — automate lead enrichment into custom data pipelines through simple AI queries


## Available Tools (6)
- **enrich_company**: Enrich a company
- **enrich_person**: Enrich a person
- **get_contact**: Get contact details
- **list_contacts**: List all contacts
- **list_exclusions**: List excluded emails
- **list_sequences**: List active sequences


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amplemarket** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Enrich the B2B contact info for 'jane.smith@example.com'."

**🤖 AI Agent:**
> Enrichment complete! For Jane Smith, I've identified a verified LinkedIn profile and her current role as 'Head of Sales'. Would you like the detailed firmographic metadata for her company?

---

**👤 You:**
> "List all active outbound sequences and their engagement rates."

**🤖 AI Agent:**
> I've retrieved your active sequences. You currently have 3 campaigns running, with 'Founder Outreach' showing a 15% reply rate. Shall I retrieve the high-fidelity detailed logs for that sequence?

---

**👤 You:**
> "Check if 'competitor.com' is on my exclusion list."

**🤖 AI Agent:**
> Scanning exclusion architecture... Yes, 'competitor.com' is currently on your opt-out list and is excluded from all automated outreach. Need help managing any other B2B exclusions?


## ❓ FAQ

**Q: How do I find my Amplemarket API Key?**
Log in to your account, navigate to **Settings** > **API**, and generate or copy your unique secret key.

**Q: Can I enrich a person using LinkedIn?**
Yes! The `enrich_person` tool allows you to provide either an email or a LinkedIn URL to retrieve the most current B2B metadata.

**Q: How do I check my exclusion list?**
Use the `list_exclusions` tool to retrieve all emails and domains currently blocked from your automated sales engagement program.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amplemarket-alternative](https://vinkius.com/mcp/amplemarket-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Amplemarket** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `amplemarket-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Amplemarket** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "amplemarket-alternative": {
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
