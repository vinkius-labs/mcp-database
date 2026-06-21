# Delighted MCP Server

Equip your AI agent to monitor customer feedback, track NPS metrics, and manage survey responses via the Delighted API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/delighted)

## Overview
**Category:** customer-support
**Tools Count:** 10

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


## Installation & Usage

To install and use the **Delighted** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/delighted](https://vinkius.com/mcp/delighted)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
