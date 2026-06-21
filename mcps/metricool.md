# Metricool MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/metricool)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Social media analytics and scheduling via Metricool — track Instagram, Facebook, and Twitter metrics.

## Description
Connect your **Metricool** account to any AI agent and take full control of your social media performance and planning through natural conversation.

### What you can do

- **Social Analytics** — Retrieve detailed metrics for Instagram, Facebook, Twitter, and LinkedIn profiles in real-time
- **Unified Summary** — Access high-level cross-channel performance reports to understand your total digital reach
- **Content Planning** — List and inspect your social media planner to stay ahead of upcoming scheduled posts
- **Ads Performance** — Monitor spend and conversion data for social advertising platforms directly from your agent
- **Profile Management** — Enumerate all connected brands and social accounts linked to your workspace

### How it works

1. Subscribe to this server
2. Enter your Metricool Access Token
3. Start managing your social strategy from Claude, Cursor, or any MCP-compatible client


## Available Tools (10)
- **get_ads_performance**: Get performance for ads
- **get_facebook_analytics**: Get Facebook analytics
- **get_instagram_analytics**: Get Instagram analytics
- **get_linkedin_analytics**: Get LinkedIn analytics
- **get_social_planner**: Get scheduled posts planner
- **get_profile_details**: Get details for a specific profile
- **get_unified_summary**: Get unified cross-channel summary
- **get_twitter_analytics**: Get Twitter analytics
- **list_published_posts**: List recently published posts
- **list_metricool_profiles**: List all connected social profiles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Metricool** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show my Instagram analytics for the last 30 days."

**🤖 AI Agent:**
> Retrieving Instagram metrics... Your profile gained 500 new followers and had 25,000 impressions this month.

---

**👤 You:**
> "What posts are scheduled in my planner?"

**🤖 AI Agent:**
> Checking your planner... You have 3 posts scheduled for tomorrow on Facebook and Instagram.

---

**👤 You:**
> "Show a summary of my performance across all channels."

**🤖 AI Agent:**
> Querying unified summary... Across all platforms, you reached 100,000 users with an average engagement rate of 4.5%.


## ❓ FAQ

**Q: How do I find my Metricool Access Token?**
Log in to Metricool, go to Account Settings > API, and you can generate or copy your Access Token there.

**Q: Can I see metrics for multiple platforms?**
Yes, Metricool supports Instagram, Facebook, Twitter, LinkedIn, and more. Use the specific tool for each platform.

**Q: Is my social media data secure?**
Absolutely. Your token is encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/metricool](https://vinkius.com/mcp/metricool)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Metricool** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `metricool` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Metricool** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "metricool": {
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
