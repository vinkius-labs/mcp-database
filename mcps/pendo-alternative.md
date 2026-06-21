# Pendo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pendo-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pendo-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pendo-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Understand product usage, guide users with in-app walkthroughs, and collect feedback that shapes your roadmap with precision.

## Description
Connect your **Pendo** account to any AI agent and take full control of your product orchestration and user engagement through natural conversation. Pendo provides a world-class platform for understanding how users interact with your software, and this integration allows you to retrieve usage metadata, manage in-app guides, and run complex aggregations directly from your chat interface.

### What you can do

- **Usage & Analytics Orchestration** — Run powerful aggregations programmatically to understand feature adoption and user behavior via natural language.
- **Metadata & Profile Control** — Update custom visitor and account metadata directly from the AI interface to ensure your CRM and success data are always synchronized.
- **Guide Lifecycle Management** — List all managed guides and retrieve detailed metadata to maintain a clear overview of your in-app messaging strategy.
- **Feature & Page Intelligence** — Access and monitor tagged features and pages to track engagement and identify bottlenecks using simple AI commands.
- **Operational Monitoring** — Track system responses and manage regional data centers (US, EU, JPN, AU) to ensure your analytics pipeline is always optimized.

### How it works

1. Subscribe to this server
2. Enter your Pendo Integration Key and regional Base URL from your settings
3. Start managing your product analytics from Claude, Cursor, or any MCP-compatible client

No more manual exporting of usage reports or context switching for user profiles. Your AI acts as a dedicated product analyst or customer success manager.

### Who is this for?

- **Product Managers** — quickly retrieve feature adoption summaries and monitor guide performance without switching apps.
- **Customer Success Teams** — automate the update of account health metadata and track visitor activity via natural conversation.
- **Growth Marketers** — streamline the retrieval of user segments and monitor engagement trends directly within the chat.


## Available Tools
- **get_pendo_account_details**: Get details for a specific account
- **get_pendo_guide_details**: Get details for a specific guide
- **get_pendo_visitor_details**: Get details for a specific visitor
- **list_pendo_features**: List tagged features
- **list_pendo_guides**: List all in-app guides
- **list_pendo_pages**: List tagged pages
- **list_reports**: List all analytics reports
- **list_segments**: List all user segments
- **run_pendo_aggregation**: Perform complex analytics and grouping
- **update_account_metadata**: Update custom account metadata
- **update_visitor_metadata**: Update custom visitor metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pendo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active in-app guides in my Pendo account."

**🤖 AI Agent:**
> I've retrieved your guides. You have 5 active environments including 'Onboarding Flow' and 'Release Announcement'. Which one would you like to see details for?

---

**👤 You:**
> "Show me the feature adoption analytics for the new dashboard module launched last month."

**🤖 AI Agent:**
> Dashboard module adoption metrics since launch (April 15): 2,847 unique visitors out of 5,200 active users (54.7% adoption). Daily active usage peaked at 1,234 on April 28. Average session duration: 4.2 minutes. Most used features: "Custom Widgets" (78% of visitors), "Data Export" (45%), "Saved Views" (34%). 3 in-app guides triggered 892 times with 67% completion rate.

---

**👤 You:**
> "List all active in-app guides and their completion metrics."

**🤖 AI Agent:**
> You have 7 active guides. "Onboarding Tour" has the highest completion at 82% (3,421 starts, 2,805 completions). "Feature Discovery" runs at 71% completion. "Upgrade Prompt" shows 45% engagement with 12% click-through to pricing. "NPS Survey" collected 1,247 responses (average score: 8.2). The lowest performer is "Advanced Settings Tour" at 38% completion, suggesting it may need simplification.


## Installation & Usage

To install and use the **Pendo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pendo-alternative](https://vinkius.com/mcp/pendo-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
