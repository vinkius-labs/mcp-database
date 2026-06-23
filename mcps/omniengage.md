# OmniEngage MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/omniengage)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Reach customers across email, SMS, push, and in-app with unified omnichannel marketing that personalizes every touchpoint.

## Description
Connect your **OmniEngage** (Cynthia AI) account to any AI agent and take full control of your sales orchestration and prospect engagement through natural conversation. OmniEngage provides a powerful platform for automated LinkedIn and email outreach, and this integration allows you to retrieve prospect metadata, launch new research sequences, and monitor campaign performance directly from your chat interface.

### What you can do

- **Prospect & Lead Orchestration** — List all managed prospects and retrieve detailed profile metadata programmatically to ensure your sales pipeline is always synchronized.
- **Campaign & Sequence Control** — Launch new outreach campaigns and trigger research sequences for prospects directly from the AI interface to drive better lead qualification.
- **Engagement Intelligence** — Access and monitor campaign results and retrieve detailed engagement metadata via natural language to maintain a high-fidelity interaction history.
- **Webhook & Automation Control** — List and oversee your configured webhooks to ensure your sales workflows are always optimized using simple AI commands.
- **Operational Monitoring** — Track system responses and manage prospect statuses to ensure your outreach strategy is always high-performing.

### How it works

1. Subscribe to this server
2. Enter your OmniEngage API Key (Bearer Token) from your dashboard settings
3. Start managing your sales outreach from Claude, Cursor, or any MCP-compatible client

No more manual status checking in the portal. Your AI acts as a dedicated sales coordinator or lead researcher.

### Who is this for?

- **Sales Development Reps (SDRs)** — quickly retrieve prospect summaries and monitor sequence health without switching apps.
- **Growth Marketers** — automate the launching of targeted outreach campaigns and track results via natural conversation.
- **Account Executives** — streamline the retrieval of lead metadata and monitor account engagement directly within the chat.


## Available Tools (12)
- **create_prospect**: Pass data as a JSON string.

Add a new prospect
- **delete_prospect**: Remove a prospect from the system
- **get_campaign_details**: Get details for a specific campaign
- **get_prospect_details**: Get specific prospect details
- **check_api_status**: Verify API connectivity and account status
- **launch_campaign**: Pass data as a JSON string.

Launch a new outreach campaign
- **list_outreach_campaigns**: List all outreach campaigns
- **list_prospects**: List all outreach prospects
- **list_sequences**: List all outreach sequences
- **list_tags**: List all prospect tags
- **list_webhooks**: List configured synchronization webhooks
- **update_prospect**: Update an existing prospect


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OmniEngage** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active prospects in OmniEngage."

**🤖 AI Agent:**
> I've retrieved your prospects. You have 25 active leads including 'John Miller' and 'Sarah Chen'. Which one would you like to see the engagement history for?

---

**👤 You:**
> "Show me details for campaign ID camp_291 including its performance stats."

**🤖 AI Agent:**
> Campaign "Spring Outreach 2025" (camp_291) has reached 342 prospects so far. Open rate stands at 47%, reply rate at 12%, and 8 meetings have been booked. The sequence includes 4 touchpoints over 14 days, and 89 prospects are still actively in the pipeline.

---

**👤 You:**
> "List all outreach sequences available in my account."

**🤖 AI Agent:**
> You have 5 active sequences. "Cold Intro" has 3 steps over 7 days, "Enterprise Follow-up" runs 5 steps across 21 days, "Re-engagement" uses 2 steps in 5 days, "Warm Lead Nurture" spans 4 steps over 10 days, and "Event Attendee" covers 3 steps in 7 days.


## ❓ FAQ

**Q: Can my AI automatically find the details for a specific prospect by their ID?**
Yes! Use the `get_prospect` tool with the Prospect ID. Your agent will respond with complete metadata for the profile, including contact info and current engagement status in seconds.

**Q: How do I find my OmniEngage API Key?**
Log in to your OmniEngage account at dashboard.omniengage.co, navigate to **Settings** > **API**, and you will find your unique secret token there.

**Q: Can I launch an outreach campaign via the AI?**
Absolutely. Use the `launch_campaign` tool. Provide the campaign data and target leads, and the agent will trigger the outreach sequence immediately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/omniengage](https://vinkius.com/mcp/omniengage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OmniEngage** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `omniengage` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OmniEngage** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "omniengage": {
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
