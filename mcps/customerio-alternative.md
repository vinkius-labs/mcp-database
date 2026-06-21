# Customer.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/customerio-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Send behavior-driven emails, push notifications, and in-app messages triggered by what your users actually do in your product.

## Description
Connect your **Customer.io** account to any AI agent and take full control of your automated lifecycle marketing and customer engagement workflows through natural conversation.

### What you can do

- **Audience Orchestration** — List and manage customer profiles programmatically, retrieving detailed attributes, traits, and segment memberships to coordinate personalized journeys
- **Segment Intelligence** — Access your complete directory of data-driven and manual segments to understand audience distributions and monitor real-time membership counts
- **Campaign Architecture** — Monitor automated marketing campaigns and retrieve high-fidelity performance reports including delivery, open, and click metrics
- **Message Dispatch** — Programmatically trigger manual broadcasts or send specific transactional emails to individuals using pre-defined message templates
- **Regional Flexibility** — Connect to both US and EU regions using specialized app API keys and regional base URLs directly through your agent

### How it works

1. Subscribe to this server
2. Retrieve your **App API Key** from Customer.io (Settings > Account Settings > API Keys)
3. Identify your **Region** (US or EU) to ensure correct endpoint routing
4. Start managing your lifecycle marketing from Claude, Cursor, or any MCP client

No more manual scrubbing through people tables or checking individual campaign logs in the portal. Your AI acts as your dedicated growth marketer and automation coordinator.

### Who is this for?

- **Growth Marketers** — instantly retrieve campaign results and check user segment memberships using natural language commands
- **Product Managers** — monitor customer engagement metrics and verify profile attributes without leaving your workspace
- **Developers & Ops** — automate transactional messaging and manage app-level metadata through simple AI queries


## Available Tools (12)
- **get_connection_status**: Check API health
- **get_campaign_performance**: Check campaign stats
- **get_customer_details**: Get person profile
- **list_segment_members**: Get people in segment
- **list_scheduled_broadcasts**: List one-to-many messages
- **list_active_campaigns**: List automated campaigns
- **list_newsletters**: List saved newsletters
- **list_customers**: io.

List audience people
- **list_audience_segments**: List user segments
- **list_transactional_messages**: g. password resets).

List 1-to-1 messages
- **send_transactional_email**: Send individual email
- **dispatch_broadcast**: Trigger manual broadcast


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Customer.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active marketing campaigns in Customer.io."

**🤖 AI Agent:**
> I've retrieved your active campaigns. You currently have 3 automated journeys running, including 'Welcome Sequence' and 'Re-engagement Flow'. Would you like the performance metrics for any of these?

---

**👤 You:**
> "Show me the audience segments and their member counts."

**🤖 AI Agent:**
> Accessing segments... Your 'Premium Users' segment has 1,240 members, and 'Trial Expired' has 450. I can provide the detailed profile attributes for specific members if needed.

---

**👤 You:**
> "Send a transactional email to 'jane@example.com' (ID: 'trans_123')."

**🤖 AI Agent:**
> Message dispatched! I've successfully triggered the transactional email 'trans_123' for Jane Doe. The delivery is now being tracked in your performance logs.


## ❓ FAQ

**Q: How do I find my Customer.io App API Key?**
Log in to Customer.io, navigate to **Settings** > **Account Settings** > **API Keys**, and select the **App API Keys** tab to generate a new token.

**Q: Does it support EU regional accounts?**
Yes! You can specify your region ('us' or 'eu') via the `CUSTOMER_IO_REGION` credential to ensure the agent connects to the correct data center.

**Q: Can I trigger a broadcast via AI?**
Yes! Use the `dispatch_broadcast` tool with a specific broadcast ID. You can optionally provide JSON parameters for Liquid data injection.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/customerio-alternative](https://vinkius.com/mcp/customerio-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Customer.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `customerio-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Customer.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "customerio-alternative": {
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
