# Google Business Profile MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-business-profile)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your local business presence — track reviews, posts, and customer Q&A via AI.

## Description
Connect your **Google Business Profile** (formerly Google My Business) account to your AI agent and take control of your local SEO and customer engagement. Use natural language to monitor reviews, reply to feedback, and update your business information across Google Search and Maps.

### What you can do

- **Location Management** — List and inspect all your business locations, including store codes and operating hours
- **Review Monitoring & Replies** — Fetch recent customer reviews and draft or post replies directly through the chat
- **Local Posts** — List and create updates, events, or offers to keep your customers informed and engaged
- **Insights & Performance** — Retrieve performance metrics to understand how customers find and interact with your business
- **Q&A Engagement** — Monitor customer questions and provide official answers to improve your profile's helpfulness

### How it works

1. Subscribe to this server
2. Enter your Google Business Account ID
3. Complete the secure Google OAuth flow to authorize management access
4. Start managing your local presence from Claude, Cursor, or any MCP-compatible client

Keep your business information up-to-date and your customers heard without manually checking the GBP dashboard every day.

### Who is this for?

- **Local Business Owners** — quickly respond to new reviews and check if your store hours are correctly listed
- **Social Media Managers** — coordinate local posts and updates across multiple storefronts via natural language
- **Customer Support Teams** — monitor and answer customer questions on Google Maps efficiently


## Available Tools
- **answer_question**: Provide an answer to a customer question
- **create_review_reply**: Reply to a customer review
- **get_location_details**: Get detailed info for a specific location
- **get_location_insights**: Fetch performance metrics for a location
- **get_review**: Get details of a specific review
- **get_verification_status**: Check verification status for a location
- **list_accounts**: List managed Google Business accounts
- **list_local_posts**: List posts (updates, events, offers) for a location
- **list_locations**: List business locations managed by the account
- **list_questions**: List customer questions for a location
- **list_reviews**: Fetch reviews for a location
- **update_business_hours**: Change business operating hours


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Business Profile** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the 5 most recent reviews for my downtown location."

**🤖 AI Agent:**
> Fetching reviews... You received 5 new reviews this week. 4 are 5-star ratings praising the service, and one is a 3-star review mentioning a wait time. Would you like me to draft a reply to the 3-star review?

---

**👤 You:**
> "Create a post about our 20% discount this weekend."

**🤖 AI Agent:**
> Drafting local post... I've prepared an 'OFFER' post with the title 'Weekend Flash Sale!' and the 20% discount details. Should I publish this to all your verified locations now?

---

**👤 You:**
> "What were the most common search terms used to find us last month?"

**🤖 AI Agent:**
> Analyzing insights... The top search terms were 'coffee near me' (1,200 searches), 'best latte in town' (850 searches), and 'breakfast cafe' (600 searches). This is a 15% increase in discovery compared to the previous month.


## ❓ FAQ

**Q: Can I respond to customer reviews directly using the AI agent?**
Yes! Use the `create_review_reply` tool. You can ask the AI to draft a professional response to a specific review and post it to your profile instantly.

**Q: How do I update my business hours for a specific holiday?**
You can use the `update_business_hours` tool. Simply provide the new hours object for the target location ID, and the agent will update your profile across Google Search and Maps.

**Q: Can I see how many people clicked 'Call' or 'Directions' on my profile?**
Yes. The `getLocationInsights` tool retrieves daily metrics, including actions like phone calls, direction requests, and website clicks initiated from your Google Business Profile.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-business-profile](https://vinkius.com/mcp/google-business-profile)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Business Profile** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `google-business-profile` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Business Profile** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-business-profile": {
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
