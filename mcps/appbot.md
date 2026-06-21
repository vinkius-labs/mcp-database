# Appbot MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/appbot)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/appbot-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/appbot-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Analyze app reviews and sentiment with Appbot — track user feedback, ratings, and topics across iOS and Android via AI.

## Description
The **Appbot MCP Server** provides deep insights into your app's user feedback. By connecting your Appbot account to your AI agent, you can programmatically retrieve reviews, analyze sentiment trends, and identify key topics from your iOS, Android, and other platform reviews using natural language.

### What you can do

- **Review Retrieval** — List and filter reviews by app, sentiment, star rating, or specific keywords.
- **Sentiment Analysis** — Quickly gauge the overall tone of user feedback (positive, negative, neutral, mixed).
- **Topic Identification** — Discover common themes in your reviews with standard and custom topics.
- **Version Tracking** — Monitor feedback for specific app versions to evaluate new releases.
- **Global Insights** — Filter reviews by country and language to understand your global audience.

### How it works

1. Subscribe to this server
2. Provide your Appbot API Key (Username) and API Secret (Password)
3. Start analyzing app reviews and user sentiment through your AI chat interface.

### Who is this for?

- **Product Managers** — Evaluate the reception of new features and identify pain points from user reviews.
- **Customer Support Leads** — Monitor sentiment and identify emerging issues before they escalate.
- **App Developers** — Track technical feedback and bug reports surfaced in app store reviews.


## Available Tools
- **get_account_info**: Retrieve Appbot account details and connection status
- **get_review_details**: Get complete details for a single specific review
- **get_reviews_by_custom_topic**: Retrieve reviews associated with a specific custom topic
- **list_apps**: List all apps tracked by your team in Appbot
- **list_countries**: List countries available for filtering reviews
- **list_custom_topics**: List user-defined custom topics set up in the Appbot dashboard
- **list_languages**: List all languages supported by Appbot for sentiment analysis
- **list_reviews**: Use sentiment, starRating, or keyword filters to narrow down the results. Useful for sentiment analysis and bug reporting.

List reviews for a specific app with optional filtering
- **list_topics**: List standard topics identified in app reviews by Appbot AI
- **list_versions**: List app versions detected in the app reviews


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Appbot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my apps tracked in Appbot."

**🤖 AI Agent:**
> I've retrieved your apps. You are currently tracking 3 apps: 'Vinkius iOS' (ID: 123), 'Vinkius Android' (ID: 456), and 'Vinkius Web' (ID: 789).

---

**👤 You:**
> "Show me the last 10 negative reviews for the iOS app."

**🤖 AI Agent:**
> I've pulled the latest 10 negative reviews. Most users are mentioning issues with the recent login update and some UI lag on older devices.

---

**👤 You:**
> "What are the most common topics in recent reviews for my Android app?"

**🤖 AI Agent:**
> The top topics for your Android app are 'Performance', 'Ease of Use', and 'Bug Reports'. 'Performance' has seen a slight increase in mentions over the last 30 days.


## Installation & Usage

To install and use the **Appbot** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/appbot](https://vinkius.com/mcp/appbot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
