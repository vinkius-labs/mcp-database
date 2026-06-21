# HeyReach MCP Server

Automate LinkedIn outreach via HeyReach — manage campaigns, leads, and connected accounts directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/heyreach)

## Overview
**Category:** sales-automation
**Tools Count:** 10

## Description
Connect your **HeyReach.io** account to any AI agent and take full control of your LinkedIn outreach and lead generation through natural conversation.

### What you can do

- **Campaign Oversight** — List all outreach campaigns, monitor their status, and pause or resume them as needed.
- **Lead Management** — Import new leads from LinkedIn profile URLs and retrieve detailed prospect information.
- **Account Visibility** — List all connected LinkedIn accounts (senders) and monitor which profile is driving your outreach.
- **Inbox Automation** — Access recent conversations and send replies directly from the chat interface.
- **Campaign Tracking** — Check which campaigns a specific lead is part of to ensure consistent communication.
- **Operational Efficiency** — Add up to 100 leads to a campaign in a single high-throughput request.

### How it works

1. Subscribe to this server
2. Enter your HeyReach API Key (found in Settings > API)
3. Start managing your LinkedIn outreach from Claude, Cursor, or any MCP-compatible client

No more manual configuration in the web dashboard for every lead import. Your AI assistant acts as a dedicated LinkedIn Outreach Manager or B2B Growth Specialist.

### Who is this for?

- **Lead Generation Agencies** — instantly trigger campaign actions and manage multiple client sender accounts.
- **SDRs & BDRs** — automate the process of adding identified prospects to relevant sequences.
- **Sales Teams** — monitor LinkedIn inbox conversations and respond directly from the sales communication flow.


## Available Tools
- **add_leads_to_campaign**: Pass the leads array as a JSON string in "leads_json" (e.g., [{"firstName": "John", "lastName": "Doe", "profileUrl": "..."}]).

Import new leads into a specific campaign
- **get_lead_details**: Get detailed information about a lead using their LinkedIn profile URL
- **get_api_profile**: Check API key validity and get basic account info
- **list_linkedin_accounts**: Use this to identify which account is sending messages.

List all LinkedIn accounts (senders) connected to the workspace
- **list_campaigns**: Use this to find the "campaignId" for adding leads or managing status.

List all LinkedIn outreach campaigns
- **list_conversations**: List recent LinkedIn inbox conversations
- **list_lead_campaigns**: List all campaigns a specific lead is part of
- **pause_campaign**: Pause an active LinkedIn campaign
- **resume_campaign**: Resume a paused LinkedIn campaign
- **send_linkedin_message**: Pass the payload as a JSON string in "body_json" (requires conversationId and text).

Send a message to a LinkedIn conversation


## Installation & Usage

To install and use the **HeyReach** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/heyreach](https://vinkius.com/mcp/heyreach)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
