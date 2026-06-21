# AppTweak MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apptweak)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Bring App Store Optimization (ASO) to your AI agent — track app rankings, fetch keyword volumes, and analyze competitor downloads via chat.

## Description
Connect your **AppTweak** account to your AI agent to unlock enterprise-grade App Store Optimization (ASO) directly from your chat workflow. Skip the heavy dashboards and ask your agent to fetch keyword intelligence, track competitor movements, and monitor your app's reviews in real time.

### What you can do

- **App Intelligence** — Retrieve full app metadata, category histories, and estimated downloads privately across iOS and Android stores
- **Keyword Strategy** — Request smart keyword suggestions, analyze search volumes, and track exact ranking positions for any given keyword
- **Review Sentiment** — Fetch direct user reviews and analyze aggregated sentiment to identify trending feature requests or emerging bugs
- **Market Analysis** — Pull the "Top Charts" of any category to identify leading apps and emerging market competitors instantly

### How it works

1. Subscribe to this MCP server
2. Securely insert your AppTweak API Key
3. Start dictating market research requests to Claude, Cursor, or any compatible conversational AI client

### Who is this for?

- **ASO Specialists** — prompt the AI to find high-volume, low-difficulty keywords without leaving your spreadsheet planning
- **Product Managers** — request an aggregated summary of the past 50 negative reviews to quickly spot major app-breaking bugs
- **User Acquisition Leads** — monitor top chart movements and track competitor estimated downloads during key seasonal campaigns
- **Founders** — get a morning digest of your current category ranking and keyword efficiencies across your target markets


## Available Tools
- **get_app_metadata**: Provide either the Apple App Store numeric ID or the Google Play Store package name. Identifies core app properties and performance indicators.

Get complete app metadata from AppTweak including title, developer, rating, reviews, category, and version
- **get_keyword_suggestions**: Crucial for optimizing organic search visibility on App Store and Google Play.

Get ASO keyword suggestions for an app on AppTweak
- **get_keyword_rankings**: Get keyword rankings for an app on AppTweak (position, volume, KEI)
- **get_keyword_volume**: Useful to find "sweet spot" keywords with high volume and low difficulty.

Get search volume and difficulty for a specific AppTweak keyword
- **get_category_rankings**: Helps diagnose the impact of feature updates or acquisition campaigns.

Get app category ranking history from AppTweak
- **get_app_reviews**: Valuable for sentiment analysis, feature requests, and bug reports from actual users.

Get app reviews from users via AppTweak
- **get_review_stats**: Good for high-level app health.

Get review statistics from AppTweak (rating distribution, sentiment)
- **get_top_charts**: Get top charts for a category via AppTweak (top free/paid/grossing apps)
- **get_download_estimates**: Essential for competitor analysis.

Get estimated download numbers for an app from AppTweak


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AppTweak** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the general App Store metadata for Spotify (ID: 324684580)."

**🤖 AI Agent:**
> Analyzed Spotify (324684580) on Apple Store (US). It ranks strongly in the 'Music' category with an average rating of 4.8 from 24 million reviews. The current version highlights a UI update. Should I fetch the recent Top Reviews or suggest keyword improvements for them?

---

**👤 You:**
> "Find 5 good keyword suggestions for a 'Habit Tracker' app and get their volume and difficulty."

**🤖 AI Agent:**
> Here are 5 analyzed keywords in the 'Habit Tracker' niche. 1) 'daily planner' — Vol: 65, Diff: High. 2) 'habit forming' — Vol: 45, Diff: Low. 3) 'streak counter' — Vol: 30, Diff: Low. 4) 'goal setting' — Vol: 50, Diff: Medium. 'streak counter' has the best KEI (Difficulty to Volume ratio). I recommend adding it to your subtitle.

---

**👤 You:**
> "Can you summarize the sentiment of the last 20 Google Play reviews for Tinder?"

**🤖 AI Agent:**
> I've fetched and analyzed the latest 20 reviews. The overall sentiment is Negative (avg rating 1.9/5). Common complaints center around: 1) Account bans without explanation, 2) The high cost of 'Gold' subscriptions relative to actual matches, and 3) An increase in bot accounts in the US market over the last 72 hours.


## ❓ FAQ

**Q: Can my AI agent rewrite my app description using the keyword suggestions?**
Yes. This is the perfect use case. First, ask the agent to fetch keyword suggestions and volume for your App ID. Then, in the same prompt, command the LLM to rewrite your 'App Store description' naturally injecting the top 5 high-KEI keywords. You get a fully optimized, data-backed description in one go.

**Q: How do I check a competitor’s downloads secretly?**
Just tell the agent to 'Get download estimates' and provide the target app ID (either Google package name or Apple ID). The agent uses AppTweak's proprietary machine learning algorithms to return a calculated daily or monthly download figure for that specific competitor without alerting them.

**Q: Are keyword volumes valid for non-US countries?**
Yes. Most AppTweak query tools require a `country` parameter. You can tell your agent to 'Check keyword rank in Brazil (br)' or 'France (fr)'. The AI automatically routes the localization tag so you get data isolated precisely for your target demographic.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apptweak](https://vinkius.com/mcp/apptweak)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AppTweak** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `apptweak` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AppTweak** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "apptweak": {
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
