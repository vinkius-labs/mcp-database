# AppFollow MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/appfollow)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage app reviews and rankings with AppFollow — track sentiment, ratings, and store charts via AI.

## Description
The **AppFollow MCP Server** brings powerful app store intelligence directly to your AI agent. Monitor your app's reputation, track your position in the charts, and analyze user feedback across all major app stores with ease.

### Key Features

- **Review Management** — List and search for user reviews across different countries and languages.
- **AI & Sentiment Analysis** — Get AI-generated summaries of user feedback and analyze the overall sentiment of your reviews.
- **Ranking Tracker** — Monitor your app's performance in store charts and track daily changes in visibility.
- **Rating Metrics** — Access current star rating distributions and historical rating trends over time.
- **App Information** — Retrieve detailed metadata and store information for any app on the market.
- **Competitive Benchmarking** — Compare your app's performance against competitors using global store data.

### Benefits for Teams

- **Customer Support** — Quickly identify common user issues and bugs reported in reviews.
- **Product Managers** — Use AI summaries to understand user sentiment and prioritize feature requests.
- **Growth & Marketing** — Track rankings and ratings to measure the effectiveness of your ASO and UA efforts.


## Available Tools (8)
- **get_account_check**: Verify AppFollow account connection
- **get_app_info**: Retrieve basic information about an app from AppFollow
- **get_rankings**: Track app rankings in store charts
- **get_ratings_history**: Get historical rating data over a period of time
- **get_ratings**: Get current star rating distribution
- **get_reviews_ai_summary**: Get an AI-generated summary of recent user reviews
- **get_reviews_summary**: Get a summary of reviews and average rating
- **list_reviews**: List app reviews for a specific app store product


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AppFollow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the most recent 1-star reviews for my app?"

**🤖 AI Agent:**
> I've found 5 recent 1-star reviews. Most users are complaining about a slow loading time after the latest update.

---

**👤 You:**
> "Give me an AI summary of user feedback for 'com.example.app'."

**🤖 AI Agent:**
> Based on the recent 100 reviews, users generally love the ease of use, but several are requesting a dark mode and better offline support.

---

**👤 You:**
> "Where does my app rank in the 'Health & Fitness' category in the US today?"

**🤖 AI Agent:**
> Your app is currently ranked #12 in 'Health & Fitness' in the United States, up 2 spots from yesterday.


## ❓ FAQ

**Q: How do I find my AppFollow API Token?**
You can find your API token in your AppFollow account settings under the **API** or **Integrations** section.

**Q: What is an 'extId' in AppFollow?**
The `extId` is the external ID of the app in the store. For iOS apps, it's the numeric Apple ID. For Google Play apps, it's the bundle name (e.g., `com.example.app`).

**Q: Does this integration support semantic tags?**
Yes, you can use the `get_reviews_semantic` tool to retrieve reviews categorized by their content type, such as 'Bug', 'Feature Request', or 'Pricing'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/appfollow](https://vinkius.com/mcp/appfollow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AppFollow** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `appfollow` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AppFollow** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "appfollow": {
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
