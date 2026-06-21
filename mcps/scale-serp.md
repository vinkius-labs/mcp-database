# Scale SERP MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/scale-serp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent with real-time Google Search data — run organic, news, shopping, and scholar queries effortlessly.

## Description
Connect **Scale SERP** to any AI agent to unlock the full power of real-time Google search data. Enable your AI to browse the web intelligently without worrying about anti-bot measures or complex scraping logic.

### What you can do

- **Comprehensive Web Search** — Execute real-time Google queries across text, images, videos, and news localized to specific geographic regions
- **E-commerce & Local** — Scrape Google Shopping results for pricing data or Google Places for local business intelligence
- **Research & SEO** — Run predictive auto-complete lookups, extract "People Also Ask" related questions, and pull scholarly articles via Google Scholar
- **Advanced Customization** — Pass raw JSON options to emulate exact languages, devices, or custom search parameters directly from your agent

### How it works

1. Subscribe to this server
2. Enter your Scale SERP API Key
3. Instantly browse Google search results programmatically from Claude, Cursor, or your preferred MCP client

Scale SERP handles the IP rotation and CAPTCHAs, allowing your agent to simply request structured data effortlessly.

### Who is this for?

- **SEO Specialists & Marketers** — track ranking positions, analyze competitors' "People Also Ask" clusters, and explore autocomplete trends
- **Researchers** — command your AI to gather Google Scholar citations and synthesize multiple papers automatically
- **Web Scrapers & Analysts** — track Google Shopping price changes across a massive array of queries without server maintenance


## Available Tools (10)
- **custom_search**: Performs a highly customized Google search
- **google_autocomplete**: Retrieves Google search autocomplete suggestions
- **google_images**: Searches for images on Google
- **google_news**: Searches for news articles on Google News
- **google_organic**: You can specify a query and an optional geographic location.

Performs a standard Google organic search
- **google_places**: Searches for places and local businesses on Google Maps
- **google_related_questions**: Retrieves "People Also Ask" questions from Google
- **google_scholar**: Searches for scholarly articles and research papers
- **google_shopping**: Searches for products on Google Shopping
- **google_videos**: Searches for videos on Google


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Scale SERP** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Run a Google Scholar search for 'machine learning in agriculture' and summarize the top 3 papers."

**🤖 AI Agent:**
> I've fetched the top results from Google Scholar. Here are the summaries of the top 3 highly cited papers from the last 5 years: 
1) 'Deep Learning for Crop Yield Prediction' - explores neural networks analyzing satellite images. 
2) 'Smart Agriculture Frameworks' - discusses IoT sensors combined with ML. 
3) 'Pest Detection models' - focuses on computer vision models to identify crop diseases.

---

**👤 You:**
> "Find restaurants near Times Square via Google Places."

**🤖 AI Agent:**
> I retrieved 5 top-rated restaurants near Times Square from Google Places: Carmine's Italian (4.5 stars, 12K reviews), Junior's Restaurant (4.4 stars), Joe's Pizza (4.6 stars), Le Bernardin (4.9 stars) and The View Restaurant (4.2 stars). Should I lookup their addresses?

---

**👤 You:**
> "Search Google for 'best CRM tools'."

**🤖 AI Agent:**
> I performed an organic Google Search. The current top ranking pages are: 1. Salesforce's 'What is CRM' portal. 2. HubSpot's Complete Guide for 2024. 3. Forbes Advisor 'Best CRM Software of The Year'. Would you like me to fetch the SEO titles or visit any of the URLs?


## ❓ FAQ

**Q: Can the AI generate content ideas by analyzing Google 'Related Questions'?**
Yes. This is a very common SEO workflow. You can prompt the agent: 'Find the related questions for "how to bake sourdough" and write a blog outline covering them'. The agent uses `google_related_questions` to pull the PAA (People Also Ask) boxes directly from Google and drafts your content.

**Q: Is it possible to track market prices in Google Shopping?**
Absolutely. You can run the `google_shopping` tool with a product query like 'iPhone 15 Pro 256GB'. Scale SERP will return the top structured shopping results, allowing the AI to summarize the lowest, highest, and median prices for you instantly.

**Q: How does the agent do location-aware searches?**
When using `google_organic` or `custom_search`, you can specify a location (e.g., 'London, UK' or a specific GL country code). Scale SERP ensures the query is routed exactly as if you were physically browsing from that region, avoiding default IP bias.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/scale-serp](https://vinkius.com/mcp/scale-serp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Scale SERP** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `scale-serp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Scale SERP** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "scale-serp": {
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
