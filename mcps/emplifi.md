# Emplifi MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/emplifi)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Equip your AI agent to manage social profiles, track post metrics, and monitor care automation via the Emplifi API.

## Description
Integrate **Emplifi**, the unified customer experience (CX) platform, directly into your AI workflow. Manage your social media profiles across platforms, track real-time post engagement and performance metrics, monitor social listening dashboards and influencer impact, and oversee your customer care automation using natural language.

### What you can do

- **Social Profile Oversight** — List and retrieve detailed information for all your managed social media accounts and profiles.
- **Performance Intelligence** — Monitor social post metrics, resolving impressions, engagement rates, and platform-specific reactions.
- **CX Automation Management** — Access and monitor customer care automation rules and workflows, tracking active statuses and triggers.
- **Experience Auditing** — Retrieve high-level summaries of social performance, listening trends, and organizational CX health instantly.

### How it works

1. Connect the Emplifi integration to your AI assistant.
2. Authorize using your Emplifi API Key (found in your account settings).
3. Orchestrate your social media strategy and customer engagement through intuitive conversation.

### Who is this for?

- **Social Media Managers** — Quickly check post performance and engagement rates on the go.
- **Customer Care Leads** — Research automation rules and team member roles via chat during workflow optimization.
- **Operations Teams** — Monitor social listening trends and organizational CX metadata instantly.


## Available Tools (10)
- **get_emplifi_account_metadata**: Retrieve metadata and limits for your Emplifi account
- **get_influencer_performance_stats**: Get performance metrics for a specific influencer/creator
- **get_social_post_metrics**: Get engagement and performance metrics for a specific social post
- **quick_cx_health_audit**: Retrieve a high-level summary of social performance and care automation
- **list_care_automation_rules**: List all customer care automation rules and workflows
- **list_content_classification_labels**: List all labels used for content classification and reporting
- **list_listening_dashboards**: List all social listening dashboards and topics
- **list_social_posts**: List recent social media posts for a specific profile
- **list_social_profiles**: List all social media profiles managed in your Emplifi account
- **list_organization_team_members**: List all team members and their roles in the organization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Emplifi** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all managed social media profiles."

**🤖 AI Agent:**
> I've found 5 social profiles, including 'Global Instagram', 'Corporate LinkedIn', and 'Support Twitter'. Would you like to see the recent post metrics for Global Instagram?

---

**👤 You:**
> "Show me metrics for social post ID 'POST-12345'."

**🤖 AI Agent:**
> Post ID 'POST-12345' has 12,500 impressions, an engagement rate of 4.2%, and 850 total reactions. It is currently your top-performing post this week. Should I compare this to your average engagement?

---

**👤 You:**
> "Check active customer care automation rules."

**🤖 AI Agent:**
> You have 3 active rules: 'Auto-reply to Mentions', 'Urgent Ticket Escalation', and 'Weekend Out-of-Office'. All are functioning normally. Would you like to see the trigger conditions for Urgent Ticket Escalation?


## ❓ FAQ

**Q: How do I get an Emplifi API Key?**
Log in to your Emplifi dashboard, navigate to **Settings > API Management**, and you can generate or retrieve your unique API Key from there. API access usually depends on your specific Emplifi package.

**Q: Can the agent publish new social posts?**
This integration currently focuses on listing and auditing social profiles, posts, and performance metrics. Scheduling or publishing new content should be managed via the Emplifi Publisher or mobile app.

**Q: Does the integration show sentiment analysis?**
While you can retrieve post metrics and listening dashboard summaries, detailed sentiment analysis and natural language processing results should be explored within the Emplifi Listening and Insights modules.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/emplifi](https://vinkius.com/mcp/emplifi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Emplifi** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `emplifi` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Emplifi** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "emplifi": {
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
