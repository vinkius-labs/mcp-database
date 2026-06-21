# Klaviyo (Marketing Automation) MCP Server

Manage your B2C CRM via Klaviyo — create profiles, track email campaigns, and audit automation flows.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/klaviyo-marketing-automation)

## Overview
**Category:** growth-engine
**Tools Count:** 10

## Description
Connect your **Klaviyo** account to any AI agent and take full control of your e-commerce marketing, customer data, and automation flows through natural conversation.

### What you can do

- **Profile Management** — Create and retrieve detailed customer profiles, including contact information, custom properties, and predictive analytics directly from your agent
- **Campaign Tracking** — List all email campaigns and retrieve detailed performance metadata, targeted audiences, and scheduled send times securely
- **Automation Flows** — Monitor your automated email and SMS sequences, including entry triggers and chronological action steps to ensure your lifecycle marketing is running smoothly
- **Audience Segmentation** — List dynamic segments and static lists to understand your customer distribution and identify high-value cohorts
- **List Orchestration** — Add existing profiles to specific marketing lists to manage subscription preferences and targeted messaging natively
- **Data Audit** — Extract comprehensive traits and behavioral analytics for specific profile IDs to power personalized customer interactions

### How it works

1. Subscribe to this server
2. Enter your Klaviyo Private API Key
3. Start managing your marketing automation from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Marketers** — track campaign statuses and audit automation flows through natural conversation without manual dashboard searching
- **Growth Engineers** — verify audience segments and monitor profile custom properties to ensure accurate data mapping
- **Business Owners** — get rapid summaries of recent campaign performances and customer base growth across multiple Klaviyo accounts


## Available Tools
- **list_profiles**: This tool is used to browse your customer base and obtain profile IDs, email addresses, and names. Use this as a starting point to find specific customers before performing detailed audits or adding them to lists.

List Klaviyo profiles (contacts)
- **get_profile**: Returns everything from contact info (email, phone, address) to custom e-commerce properties, predictive analytics (CLV, churn risk), and marketing preferences.

Get a Klaviyo profile by ID
- **create_profile**: This is essential for manual lead insertion or synchronizing data from other sources. Requires an email address; first and last names are optional but recommended for personalization.

Create a new Klaviyo profile
- **list_lists**: Use this to identify target lists for profile orchestration or to audit your subscription groups. Returns list IDs, names, and total contact counts.

List all Klaviyo audience lists
- **add_profiles_to_list**: This tool is critical for managing subscriptions and segmenting customers for specific marketing campaigns. Input profile IDs as a comma-separated string.

Add profiles to a Klaviyo list
- **list_email_campaigns**: This tool allows you to monitor marketing activity, check which campaigns are currently active, and see scheduled send times for upcoming broadcasts.

List Klaviyo email campaigns
- **get_campaign_details**: Returns its current status (draft, sent, scheduled), the targeted audience list/segment IDs, and the message content being delivered.

Get details for a Klaviyo campaign
- **list_automation_flows**: Use this to audit your automated lifecycle marketing, such as welcome series, abandoned carts, or post-purchase follow-ups. Returns flow IDs, names, and active status.

List Klaviyo automation flows
- **get_flow_details**: It returns the entry trigger conditions, the sequence of action steps (emails, SMS, delays), and the current operational status of the automation.

Get details for a Klaviyo automation flow
- **list_audience_segments**: Unlike lists, segments update automatically based on behavioral data and predictive analytics. Use this to understand your high-value customers, churn risks, or engaged subscribers.

List Klaviyo audience segments


## Installation & Usage

To install and use the **Klaviyo (Marketing Automation)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/klaviyo-marketing-automation](https://vinkius.com/mcp/klaviyo-marketing-automation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
