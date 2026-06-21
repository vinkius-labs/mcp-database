# Ometria Email Events MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ometria-email-events)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ometria-email-events-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ometria-email-events-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Track and analyze email engagement events via Ometria — monitor opens, clicks, and bounces directly from your AI agent.

## Description
Connect your **Ometria** account to your AI agent and gain granular visibility into your email marketing performance through real-time event tracking and natural conversation.

### What you can do

- **Event Monitoring** — List and inspect raw email engagement events including opens, clicks, and delivery statuses.
- **Deliverability Insights** — Access detailed logs of email bounces and spam complaints to monitor your sender reputation.
- **Opt-out Tracking** — Monitor unsubscribe events to keep your audience lists clean and compliant.
- **Contact-level Analytics** — Retrieve the full email engagement history for any specific customer or contact ID.
- **Campaign Attribution** — List all engagement events associated with a specific marketing campaign.
- **Real-time Oversight** — Fetch the most recent email events to track live campaign launches.
- **Deep Inspection** — Fetch complete metadata and timestamps for any specific email event using its unique ID.

### How it works

1. Subscribe to this server
2. Enter your Ometria API Key (X-Ometria-Auth)
3. Start exploring email engagement intelligence from Claude, Cursor, or any MCP client

### Who is this for?

- **Email Marketers** — quickly check campaign open/click trends or deliverability issues without opening the portal.
- **Customer Success** — verify if a customer has received and opened critical communication before a call.
- **CRM Managers** — monitor engagement signals and unsubscribe trends through natural language.


## Available Tools
- **get_event_details**: Get specific event info
- **list_email_bounces**: List email bounce events
- **list_email_clicks**: List email click events
- **list_email_complaints**: List email spam complaints
- **list_events_by_campaign**: List events for a specific campaign
- **list_events_by_contact**: List events for a specific contact
- **list_email_events**: ) from Ometria.

List all email engagement events
- **list_email_opens**: List email open events
- **list_recent_email_events**: List most recent email events
- **list_email_unsubscribes**: List email unsubscribe events


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ometria Email Events** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all email open events from the last hour."

**🤖 AI Agent:**
> Retrieving recent opens... I found 45 open events in the last hour. Most activity is coming from the 'Holiday Special' campaign. Would you like to see which specific links were clicked as well?

---

**👤 You:**
> "How many bounces occurred in campaign 'camp_98765'?"

**🤖 AI Agent:**
> Checking campaign events... Campaign camp_98765 recorded 12 bounces. 8 were 'Permanent' (hard bounces) and 4 were 'Transient'. Shall I list the contact emails that hard bounced so you can clean your list?

---

**👤 You:**
> "Show me the email engagement history for 'john@example.com'."

**🤖 AI Agent:**
> Fetching contact history... John Smith (john@example.com) has a very active history: 12 opens and 5 clicks across 3 campaigns in the last 30 days. He recently clicked a link in the 'Loyalty Rewards' email. Would you like the full timestamped log?


## Installation & Usage

To install and use the **Ometria Email Events** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ometria-email-events](https://vinkius.com/mcp/ometria-email-events)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
