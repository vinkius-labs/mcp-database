# Outreach MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/outreach-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Execute sales engagement sequences with emails, calls, and social touches orchestrated by AI to maximize rep productivity.

## Description
Connect your **Outreach.io** account to any AI agent and take full control of your sales orchestration and prospect engagement through natural conversation. Outreach is the premier sales engagement platform, and this integration allows you to retrieve prospect metadata, enroll leads into automated sequences, and monitor mailing performance directly from your chat interface.

### What you can do

- **Prospect & Audience Orchestration** — List all managed prospects and retrieve detailed profile metadata programmatically to ensure your sales database is always synchronized.
- **Sequence & Automation Control** — Enroll prospects into automated sequences and monitor sequence states directly from the AI interface to track lead nurturing progress.
- **Communication Intelligence** — Access and monitor sent mailings and retrieve detailed engagement metadata via natural language to drive better follow-up efficiency.
- **Account & Deal Oversight** — Access organizational accounts and monitor sales opportunities using simple AI commands to maintain a clear overview of your pipeline.
- **Operational Monitoring** — Track system responses and manage sales tasks to ensure your outreach workflows are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Outreach.io OAuth2 Access Token from your developer portal
3. Start managing your sales engagement from Claude, Cursor, or any MCP-compatible client

No more manual status checking in the CRM. Your AI acts as a dedicated sales operations lead or engagement coordinator.

### Who is this for?

- **SDRs & BDRs** — quickly retrieve prospect summaries and monitor sequence health without switching apps.
- **Sales Managers** — automate the retrieval of mailing stats and track team productivity via natural conversation.
- **Growth Marketers** — streamline the retrieval of account metadata and monitor pipeline health directly within the chat.


## Available Tools
- **add_to_sequence**: Enroll prospect in sequence
- **create_prospect**: Add new prospect
- **get_user_info**: Get account profile
- **get_prospect_details**: Get full prospect info
- **list_companies**: List outreach accounts
- **list_sent_emails**: List sent mailings
- **list_opportunities**: List sales deals
- **list_prospects**: List engageable people
- **list_sequences**: List sales sequences
- **list_sales_tasks**: List pending actions
- **list_email_templates**: List message templates
- **update_prospect**: Modify prospect info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Outreach** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active prospects in Outreach."

**🤖 AI Agent:**
> I've retrieved your prospects. You have 25 active leads including 'John Miller' from Acme Corp and 'Sarah Chen'. Which one would you like to see sequence details for?

---

**👤 You:**
> "Show me all active email sequences and their open rates for this quarter."

**🤖 AI Agent:**
> You have 8 active sequences this quarter. "Enterprise Cold Outreach" leads with a 52% open rate across 1,240 prospects. "Product Launch Follow-up" has 47% opens and 14% replies. Your lowest performer is "Re-engagement Q1" at 23% opens, which may benefit from subject line optimization.

---

**👤 You:**
> "Find all prospects who replied positively to the Enterprise sequence in the last 7 days."

**🤖 AI Agent:**
> 14 prospects replied positively to "Enterprise Cold Outreach" in the past week. Notable responses include Maria Chen (VP Engineering at DataFlow), who requested a demo for next Tuesday, and James Park (CTO at ScaleUp), who asked for pricing details. 5 prospects were automatically moved to your "Meeting Booked" stage.


## ❓ FAQ

**Q: Can my AI automatically find the details for a specific prospect by their ID?**
Yes! Use the `get_prospect` tool with the Prospect ID. Your agent will respond with complete metadata for the record, including custom fields, sequence history, and owner info in seconds.

**Q: How do I find my Outreach.io OAuth2 Access Token?**
Log in to your Outreach Developer Portal, create a new **App**, and use the provided client credentials to perform the OAuth 2.0 flow to obtain a secret access token.

**Q: Does this work with the Outreach API v2?**
Yes, this MCP server is specifically built using the Outreach JSON:API v2 specification to ensure full compatibility with modern sales workflows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/outreach-alternative](https://vinkius.com/mcp/outreach-alternative)
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
3. Set Type to "SSE", enter `outreach-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Outreach** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "outreach-alternative": {
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
