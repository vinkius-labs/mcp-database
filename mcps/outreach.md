# Outreach MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/outreach)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Equip your AI agent with direct access to Outreach — manage prospects, track sequences, and analyze sales engagement without opening the Outreach platform.

## Description
Connect **Outreach** to your AI agent and manage your enterprise sales engagement platform conversationally.

### What you can do

- **Prospect Management** — Search, create, and update prospect records with contact information, tags, and engagement history.
- **Sequence Tracking** — List active sequences, check enrollment statuses, and monitor step completion rates.
- **Email Analytics** — Pull open rates, reply rates, bounce rates, and click metrics across sequences and campaigns.
- **Activity Feed** — Query recent calls, emails, and tasks across your SDR team for pipeline visibility.

### How it works

1. Subscribe to the Outreach integration on the marketplace.
2. Create an OAuth app in the Outreach Developer Portal (developers.outreach.io → My Apps → Create New App).
3. Ask your AI agent to manage prospects, track sequences, or pull engagement data.

### Who is this for?

- **SDR Teams** — Monitor sequence performance and prospect engagement without leaving the coding environment.
- **Sales Managers** — Get instant visibility into team activity, sequence effectiveness, and pipeline health.
- **Revenue Operations** — Pull engagement data for reporting, forecasting, and process optimization.


## Available Tools (8)
- **get_outreach_prospect**: Get details for a specific prospect
- **get_outreach_sequence_stats**: Get engagement metrics for a sequence
- **list_outreach_accounts**: List company accounts
- **list_outreach_emails**: List email addresses linked to prospects
- **list_outreach_mailboxes**: List connected sending mailboxes
- **list_outreach_prospects**: List sales prospects
- **list_outreach_sequences**: List automated outreach sequences
- **list_outreach_tasks**: List sales tasks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Outreach** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How are my active sequences performing?"

**🤖 AI Agent:**
> You have 5 active sequences. Top performer: 'VP Sales Outreach' (42% open rate, 12% reply rate, 3 meetings booked this week). Lowest: 'Cold Inbound Re-Engage' (18% open rate, 2% reply rate). Consider pausing or revising the underperforming sequence.

---

**👤 You:**
> "Search for prospect 'David Kim' in Outreach."

**🤖 AI Agent:**
> Found: David Kim (david.kim@techcorp.com). Title: VP Engineering at TechCorp. Stage: Replied. Active in sequence 'Engineering Leaders Q2'. Last email opened 4 hours ago. 2 calls logged, 0 meetings booked.

---

**👤 You:**
> "What did my SDR team accomplish yesterday?"

**🤖 AI Agent:**
> Yesterday's team summary (8 reps): 342 emails sent, 28 calls made, 45 opens tracked, 12 replies received (4 positive), and 2 meetings booked. Top performer: Sarah M. (52 emails, 3 replies, 1 meeting).


## ❓ FAQ

**Q: How do I get my Outreach API credentials?**
Go to the **Outreach Developer Portal** at **developers.outreach.io** and log in with your Outreach account. Navigate to **My Apps** and click **Create New App**. Provide a name, description, and configure the **Redirect URI** and required **scopes** (e.g., `read_prospects`, `write_prospects`). After saving, you'll receive your **Client ID** and **Client Secret**. Copy both and paste them into the configuration fields below. Note: Outreach generates both development and production credentials — use development credentials for testing.

**Q: Can my AI agent tell me which sequences are performing best?**
Yes. Ask your agent to compare sequences by reply rate, open rate, or meeting booked rate and it returns a ranked list — helping you double down on what works and kill underperforming sequences before they damage your domain reputation.

**Q: What if I need to check team activity quickly during standup?**
Ask your AI agent 'What did my team do yesterday?' and get a summary of emails sent, calls made, replies received, and meetings booked per rep — perfect for 30-second standup updates without pulling up dashboards.

**Q: Is this suitable for large enterprise SDR teams?**
Absolutely. Outreach is built for enterprise sales organizations with hundreds of reps. Your AI agent queries the same API used by Outreach's native platform — supporting team-level views, advanced filtering, and role-based access controls.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/outreach](https://vinkius.com/mcp/outreach)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Outreach** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `outreach` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Outreach** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "outreach": {
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
