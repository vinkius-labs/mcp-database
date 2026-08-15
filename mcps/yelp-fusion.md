# Yelp Fusion MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/yelp-fusion)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel-hospitality](../categories/travel-hospitality.md)

Search for local businesses, read reviews, and explore events worldwide directly from your AI agent using Yelp's rich database.

## Description
Connect **Yelp Fusion** to your AI agent to discover the best local businesses, restaurants, and services. Access millions of reviews, photos, and business details through natural conversation.

### What you can do

- **Business Discovery** — Search for businesses by term, location, or phone number with advanced filters like price and status.
- **Rich Details & Reviews** — Fetch business metadata, operating hours, and recent review excerpts to make informed decisions.
- **Events & Highlights** — Find local events, featured happenings, and review highlights for specific venues.
- **Category Exploration** — Browse Yelp's extensive category tree to find niche services or specific cuisines.
- **Transaction Search** — Identify businesses that support food delivery or specific service offerings.

### How it works

1. Subscribe to this server
2. Enter your Yelp Fusion API Key
3. Start exploring local data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Travelers & Foodies** — Find the best-rated spots in any city without leaving your chat interface.
- **Market Researchers** — Analyze business density and review sentiment for specific categories or regions.
- **Local Service Seekers** — Quickly find contact info, delivery options, and business hours for local providers.


## Available Tools (17)
- **autocomplete**: Suggestions for businesses, keywords, and categories
- **get_business_details**: Get rich data for a specific business
- **get_business_engagement**: Get engagement metrics
- **get_business_insights**: Get monthly business insights
- **get_business_reviews**: Get up to 3 review excerpts for a business
- **get_categories**: Get all business categories
- **get_category_details**: Get details for a specific category
- **get_event_details**: Get detailed information for a specific event
- **get_featured_event**: Get the featured event for a location
- **get_jobs**: g., "plumbing") for Home Services.

Get job types based on natural language query
- **get_review_highlights**: Get a business review highlights
- **get_service_offerings**: Get active and eligible service offerings
- **match_business**: Find a Yelp business matching exact input data
- **search_businesses**: Search for businesses on Yelp
- **search_by_phone**: Must start with + and country code.

Search for businesses by phone number
- **search_events**: Search for local events
- **search_transactions**: Search for businesses supporting food delivery


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Yelp Fusion** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find highly-rated Italian restaurants in Brooklyn that are open now."

**🤖 AI Agent:**
> I've searched Yelp for Italian restaurants in Brooklyn. Top options currently open include 'L'Industrie Pizzeria' (Rating: 4.8) and 'Al Di La Trattoria' (Rating: 4.5). Would you like the address or reviews for any of these?

---

**👤 You:**
> "What are the review highlights for the business with ID 'v76-88-99'?"

**🤖 AI Agent:**
> Fetching highlights for that business... Customers frequently mention 'excellent service', 'authentic flavors', and 'great atmosphere'. There are also specific mentions of their signature pasta dish being a must-try.

---

**👤 You:**
> "Search for upcoming food events in Austin, Texas."

**🤖 AI Agent:**
> I found several upcoming events in Austin. Notable ones include the 'Austin Food & Wine Festival' and the 'Taco & Margarita Fest'. Would you like the specific dates and location details for these?


## ❓ FAQ

**Q: Can I find businesses that offer delivery in my area?**
Yes. Use the `search_transactions` tool. It specifically filters for businesses that support food delivery transactions in your specified location.

**Q: How can I see what people are saying about a specific business?**
Use the `get_business_reviews` tool with the business ID or alias. It returns up to 3 review excerpts and ratings to help you gauge the quality of the establishment.

**Q: Is it possible to identify a business using just a phone number?**
Absolutely. The `search_by_phone` tool allows you to find a Yelp business by providing its phone number (including the '+' and country code).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/yelp-fusion](https://vinkius.com/mcp/yelp-fusion)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Yelp Fusion** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `yelp-fusion` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Yelp Fusion** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "yelp-fusion": {
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
