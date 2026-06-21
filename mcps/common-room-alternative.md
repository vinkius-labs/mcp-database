# Common Room MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/common-room-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration](../categories/collaboration.md)

Unify community signals from Slack, Discord, GitHub, and social media to identify your most engaged users and advocates.

## Description
Connect your **Common Room** account to any AI agent and take full control of your community orchestration and B2B relationship intelligence through natural conversation.

### What you can do

- **Member & Identity Orchestration** — List and manage community profiles programmatically, using Person360™ technology to resolve cross-channel identities (Slack, Discord, GitHub, etc.)
- **Signal Ingestion** — Programmatically ingest custom activity signals from social platforms and internal tools to maintain a high-fidelity record of member interactions
- **Audience Segmentation** — Access and monitor community segments (Highly Engaged, At Risk, etc.) and tags to understand your community's behavioral health in real-time
- **Relationship Intelligence** — Retrieve complete directories of community members and manage detailed metadata to perfectly coordinate your go-to-market outreach
- **Compliance & Privacy** — Execute 'Right to be Forgotten' deletions programmatically and monitor API token status and webhooks directly through your agent

### How it works

1. Subscribe to this server
2. Retrieve your **API Token** from Common Room (Settings > API Tokens)
3. Start managing your community intelligence from Claude, Cursor, or any MCP client

No more manual scrubbing through fragmented social logs. Your AI acts as your dedicated community manager and relationship coordinator.

### Who is this for?

- **Community Managers** — instantly retrieve member profiles and check engagement levels using natural language commands
- **DevRel & GTM Teams** — monitor social signals across multiple channels and identify high-impact contributors without leaving your workspace
- **Operations Leads** — automate member provisioning and manage webhook configurations through simple AI queries


## Available Tools
- **create_member**: Create a new community member
- **create_webhook**: Configure a new webhook
- **delete_member**: Remove member (GDPR)
- **delete_webhook**: Delete a webhook
- **get_member**: Get member details
- **get_token_status**: Check API token status
- **ingest_activity**: g., Slack post, social interaction) into a members timeline.

Report community activity
- **list_members**: List community members
- **list_segments**: g., Highly Engaged, At Risk).

List community segments
- **list_tags**: List community tags
- **list_webhooks**: List configured webhooks
- **update_member**: Update member profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Common Room** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all members in the 'Highly Engaged' segment."

**🤖 AI Agent:**
> I've retrieved the 'Highly Engaged' segment. You have 15 members in this category, including top contributors from GitHub and Slack. Would you like the Person360 profiles for the top 3?

---

**👤 You:**
> "Get the community profile for 'john@example.com'."

**🤖 AI Agent:**
> I've located John's Person360 profile. He is active on Slack and GitHub (username: john_dev). His current sentiment is 'Positive' and he is tagged as a 'Power User'. Shall I check his latest activity signals?

---

**👤 You:**
> "Report a new Slack activity for member ID 'abc-123'."

**🤖 AI Agent:**
> Activity ingested! I've successfully registered the new Slack signal for member abc-123. The interaction is now visible in their community timeline and engagement score. Need help with other members?


## ❓ FAQ

**Q: How do I find my Common Room API Token?**
Log in to your account, navigate to **Settings** > **API Tokens**, and generate a new Bearer Token for your integration.

**Q: What is the Person360™ engine?**
Person360™ is Common Room's identity resolution engine that unifies data from multiple platforms into one single member profile.

**Q: Can the agent ingest custom social signals?**
Yes! The `ingest_activity` tool allows you to push any user interaction into a member's community timeline programmatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/common-room-alternative](https://vinkius.com/mcp/common-room-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Common Room** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `common-room-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Common Room** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "common-room-alternative": {
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
