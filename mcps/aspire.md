# Aspire MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aspire)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-advertising](../categories/marketing-advertising.md)

Manage influencer marketing campaigns and creators with Aspire — track projects, members, and content via AI.

## Description
The **Aspire MCP Server** empowers your AI agent to manage your influencer marketing and creator relationships directly from your workspace. Gain instant visibility into your campaigns, audit creator profiles, and monitor content performance using simple natural language.

### Key Features

- **Project Oversight** — List all active and archived projects/campaigns and retrieve detailed metadata for any specific initiative.
- **Creator Management** — Access profiles of creators and members associated with your projects to ensure high-quality partnerships.
- **Content Tracking** — Monitor social posts and content performance, including engagement metrics and URLs.
- **Campaign Intelligence** — Quickly analyze project statuses and brand participation without navigating complex dashboards.
- **Search & Discovery** — Use powerful tools to find specific members or posts across your entire influencer database.
- **Secure API Integration** — Uses your Aspire `X-API-Key` for safe and authenticated access to your marketing data.

### Who is this for?

- **Influencer Marketing Managers** — Quickly audit campaign progress and creator participation using natural language.
- **Social Media Strategists** — Analyze content performance and engagement rates across multiple platforms.
- **Growth Marketers** — Retrieve project data and member lists for strategic planning and ROI analysis.


## Available Tools (8)
- **get_account_check**: Verify Aspire account connection
- **get_member**: Get detailed profile for a specific creator/member
- **get_post**: Get engagement metrics for a specific post
- **get_project**: Get details for a specific project
- **list_campaigns**: Alias for list_projects. Lists marketing campaigns
- **list_posts**: List social posts and content performance
- **list_project_members**: List creators and members associated with a project
- **list_projects**: List all active and archived projects/campaigns in Aspire


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aspire** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active marketing projects in Aspire."

**🤖 AI Agent:**
> I've retrieved your active projects. You have 5 running campaigns, including 'Spring Product Launch' and 'Summer Influencer Outreach'.

---

**👤 You:**
> "Who are the creators participating in the 'Summer Outreach' project?"

**🤖 AI Agent:**
> There are 12 creators in the 'Summer Outreach' project, including @TravelExplorer and @FoodieLife. Would you like to see the profile for one of them?

---

**👤 You:**
> "Show me the engagement metrics for post ID '998877'."

**🤖 AI Agent:**
> Post '998877' has an engagement rate of 4.5%, with 1,200 likes and 85 comments so far.


## ❓ FAQ

**Q: How do I find my Aspire API Key?**
Log in to your Aspire account, navigate to **Account Settings > API Keys**, and you can generate a new API key there.

**Q: Can I see engagement rates for social posts?**
Yes, the `get_post` tool retrieves detailed metrics for specific social content, including engagement rates and other performance data.

**Q: What platforms are supported by Aspire?**
Aspire supports all major social platforms including Instagram, TikTok, YouTube, and Pinterest. If the platform is linked to your project, you can track its content.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aspire](https://vinkius.com/mcp/aspire)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aspire** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aspire` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aspire** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aspire": {
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
