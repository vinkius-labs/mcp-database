# Reply.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/replyio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Equip your AI agent with direct access to Reply.io — manage outreach campaigns, track prospect engagement, and automate multi-channel sequences without opening the Reply dashboard.

## Description
Connect **Reply.io** to your AI agent and manage your multi-channel sales engagement platform conversationally.

### What you can do

- **Campaign Management** — List, create, and pause outreach campaigns across email, LinkedIn, calls, and SMS channels.
- **Prospect Tracking** — Add prospects, check engagement statuses (opened, replied, bounced), and manage contact lists.
- **Sequence Analytics** — Pull performance metrics per campaign and per step — open rates, reply rates, and conversion data.
- **People Search** — Use Reply.io's contact database to find prospect emails and enrich your outreach lists.

### How it works

1. Subscribe to the Reply.io integration on the marketplace.
2. Get your API key from your Reply.io account (Settings → API Key → copy the key).
3. Ask your AI agent to manage campaigns, track prospects, or pull engagement data.

### Who is this for?

- **SDR Teams** — Manage outreach workflows and track prospect engagement from a single conversational interface.
- **Sales Leaders** — Monitor team-wide campaign performance and identify the best-performing sequences.
- **Growth Hackers** — Automate prospect enrichment and multi-channel outreach at scale.


## Available Tools (8)
- **list_email_accounts**: List email accounts
- **get_campaign_stats**: Get campaign stats
- **pause_person**: Pause a person
- **list_campaigns**: io outreach campaigns.

List campaigns
- **get_campaign**: Get campaign
- **list_people**: io.

List people
- **add_person**: io.

Add a person
- **resume_person**: Resume a person


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reply.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the performance of my 'CTO Outreach' campaign."

**🤖 AI Agent:**
> Campaign 'CTO Outreach': 280 prospects enrolled. Open rate: 58%. Reply rate: 11%. Bounce rate: 3%. Positive replies: 18. Best performing step: Step 2 (LinkedIn connection request) with 72% acceptance rate.

---

**👤 You:**
> "Add prospect alex@techstart.com to the 'Series B Founders' sequence."

**🤖 AI Agent:**
> Prospect added: alex@techstart.com → 'Series B Founders' sequence. Starting at Step 1 (personalized email). Next touchpoint scheduled based on your campaign timing settings.

---

**👤 You:**
> "Which prospects replied positively this week?"

**🤖 AI Agent:**
> 11 positive replies this week: 4 from 'CTO Outreach' (interested in demo), 5 from 'Series B Founders' (want pricing info), and 2 from 'VP Sales Q2' (scheduling calls). I can show you the reply content for any of them.


## ❓ FAQ

**Q: How do I get my Reply.io API key?**
Log in to your Reply.io account at **app.reply.io**. Click **Settings** in the left sidebar (gear icon). Navigate to the **API Key** section. Your API key is displayed directly on this page — click the **copy icon** to copy it. If no key exists, click **Generate API Key**. Paste it into the configuration field below. The API key has the same permissions as your user account.

**Q: Can I track LinkedIn and email engagement together?**
Yes. Reply.io's multi-channel sequences combine email, LinkedIn, calls, and SMS in a single workflow. Your AI agent can pull engagement data across all channels — showing you which touchpoints drive the most replies and converting the best for each campaign.

**Q: Can my agent find prospect emails using Reply.io's database?**
Yes. Reply.io includes a built-in contact database. Your AI agent can search by company, job title, location, and industry to find verified prospect emails — then add them directly to outreach campaigns in one conversation.

**Q: What happens if a prospect replies while I'm using the agent?**
Reply.io automatically pauses the sequence for that prospect when they reply. Your AI agent can read the reply content and status via the API — so you always have up-to-date engagement signals to decide on next steps.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/replyio](https://vinkius.com/mcp/replyio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reply.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `replyio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reply.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "replyio": {
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
