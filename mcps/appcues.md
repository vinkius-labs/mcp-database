# Appcues MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/appcues)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Manage your Appcues flows, segments, and user experiences with AI — track activity and publish content effortlessly.

## Description
The **Appcues MCP Server** empowers your AI agent to interact directly with your Appcues account. Whether you need to audit your current onboarding flows, manage user segments, or track real-time user activity, this integration provides a seamless natural language interface to your product experience platform.

### Key Features

- **Flow Management** — List, view, publish, and unpublish flows (in-app experiences) across web and mobile.
- **User Segmentation** — Retrieve and analyze your targeting segments to understand who is seeing your content.
- **Activity Tracking** — Send real-time events and profile updates for immediate targeting and personalization.
- **Mobile Support** — Access specific experiences designed for your mobile applications.
- **Auditing & Reporting** — Quickly check account status, checklists, and experience metadata.

### Benefits for Teams

- **Product Managers** — Quickly audit which onboarding flows are active and make changes without leaving your AI workspace.
- **Growth Engineers** — Programmatically track user events to trigger personalized in-app journeys.
- **Customer Success** — View user profiles and segment membership to provide better support and guidance.


## Available Tools (11)
- **get_account_details**: Verify Appcues account connection
- **get_flow**: Get details for a specific flow
- **get_segment**: Get details for a specific segment
- **get_user_profile**: Retrieve the profile of a specific user
- **list_checklists**: List all checklists configured in the account
- **list_flows**: List all Appcues flows (experiences) for the account
- **list_mobile_experiences**: List mobile-specific experiences
- **list_segments**: List all user segments defined in Appcues
- **publish_flow**: Publish a draft flow
- **track_user_activity**: Use JSON strings for profileUpdate and events.

Track real-time events and profile updates for a user
- **unpublish_flow**: Unpublish an active flow


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Appcues** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active Appcues flows."

**🤖 AI Agent:**
> I've retrieved your flows. You have 5 active flows, including 'New User Onboarding', 'Feature Announcement v2', and 'NPS Survey'.

---

**👤 You:**
> "Track a 'clicked_checkout' event for user 'user_123'."

**🤖 AI Agent:**
> The 'clicked_checkout' event has been successfully tracked for user 'user_123'.

---

**👤 You:**
> "Show me the details of the segment with ID '998877'."

**🤖 AI Agent:**
> Segment '998877' is named 'High Value Customers' and currently contains 1,250 users.


## ❓ FAQ

**Q: How do I get my Appcues API Key and Secret?**
You can generate API keys in the Appcues Studio. Go to **Settings > Integrations > API Keys** to create a new set of credentials.

**Q: What is my Appcues Account ID?**
Your Account ID is a unique numeric identifier for your Appcues account. You can find it in the URL of your Appcues Studio (e.g., studio.appcues.com/accounts/YOUR_ID) or in your Account Settings.

**Q: Does this server support the EU region?**
Yes, you can configure the `APPCUES_REGION` environment variable to `eu` if your account is hosted in the Appcues European data center.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/appcues](https://vinkius.com/mcp/appcues)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Appcues** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `appcues` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Appcues** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "appcues": {
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
