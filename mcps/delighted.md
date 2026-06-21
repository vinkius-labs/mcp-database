# Delighted MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/delighted)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/delighted-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/delighted-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Equip your AI agent to monitor customer feedback, track NPS metrics, and manage survey responses via the Delighted API.

## Description
Integrate **Delighted by Qualtrics**, the leading experience management platform, directly into your AI workflow. Monitor your customer feedback in real-time, track Net Promoter Score (NPS) metrics, and analyze survey comments using natural language.

### What you can do

- **Feedback Monitoring** — List and retrieve detailed survey responses, including scores and text comments from your customers.
- **Metric Intelligence** — Retrieve overall NPS metrics, including promoter, passive, and detractor counts.
- **Customer Research** — Access feedback history and metadata for specific individuals in your database.
- **Survey Automation** — Add new people to Delighted to trigger feedback surveys directly via chat.

### How it works

1. Connect the Delighted integration to your AI assistant.
2. Authorize using your Delighted API Key (found in your account settings).
3. Gain real-time insights into customer satisfaction through intuitive conversation.

### Who is this for?

- **Customer Experience (CX) Leads** — Quickly identify promoters and detractors on the go.
- **Product Managers** — Search for specific feedback themes and comments to inform product roadmaps.
- **Support Teams** — Review customer feedback history before resolving support tickets.


## Available Tools
- **add_person_to_survey**: Adds a new person to the system and schedules a survey invitation to be sent via the default channel.

Add a new person to Delighted to trigger a survey
- **get_nps_metrics_summary**: Returns real-time Net Promoter Score (NPS) along with a breakdown of promoters, passives, and detractors.

Retrieve overall NPS metrics, including promoter and detractor counts
- **get_person_feedback_history**: Resolves all previous survey responses, cumulative NPS contribution, and associated person attributes.

Get all feedback and metadata for a specific person
- **get_recent_customer_comments**: List the most recent survey responses that include a text comment
- **get_response_details**: Resolves customer details, specific survey channel, and the full text of the feedback comment.

Get full details for a specific survey response
- **list_recent_detractors**: Identifies "detractors" based on an NPS score between 0 and 6.

Identify customers who provided a low NPS score (0-6)
- **list_feedback_contacts**: Returns a list of people who have interacted with Delighted, including their email addresses and survey history metadata.

List people who have been sent surveys or provided feedback
- **list_top_promoters**: Identifies "promoters" based on an NPS score of 9 or 10.

Identify customers who provided a high NPS score (9-10)
- **list_survey_responses**: Returns response metadata including score, comment, person identifier, and timestamp.

List all customer survey responses in Delighted
- **search_responses_by_comment**: Identifies survey responses where the text matches the provided search term.

Search for survey responses containing specific keywords in comments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Delighted** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is our current NPS score?"

**🤖 AI Agent:**
> Your current NPS score is 58. You have 120 Promoters, 45 Passives, and 15 Detractors based on recent survey responses. Would you like to see the latest comments from detractors?

---

**👤 You:**
> "Show me the last 5 customer comments containing 'pricing'."

**🤖 AI Agent:**
> I've found 5 recent comments related to pricing. Highlights include: 'Value is great for the price' and 'A bit expensive compared to competitors'. Should I pull the full text for all of them?

---

**👤 You:**
> "Get the feedback history for 'user@example.com'."

**🤖 AI Agent:**
> I've retrieved the history for 'user@example.com'. They have provided 3 responses over the last year, with scores of 10, 9, and 10. Their most recent comment was 'Excellent support experience!'. Would you like to see their custom properties?


## Installation & Usage

To install and use the **Delighted** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/delighted](https://vinkius.com/mcp/delighted)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
