# Zoho Campaign MCP Server

AI email marketing: manage campaigns, contacts, and mailing lists via agents.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-campaign)

## Overview
**Category:** marketing-automation
**Tools Count:** 13

## Description
### What you can do

Supercharge your email marketing with AI agents controlling Zoho Campaign. Automate your entire workflow:

- **Create and manage email campaigns** with custom subjects, senders, and mailing lists
- **Review campaign analytics** including opens, clicks, bounces, and unsubscribes
- **Build and segment mailing lists** for targeted audience reach
- **Import and export contacts** with bulk add/remove operations
- **Track contact engagement** and subscription status across all lists
- **Monitor blocked contacts** to maintain list hygiene and deliverability

### How it works

1. **Connect your Zoho Campaign account** via OAuth token from Zoho API Console
2. **Ask your AI agent** to create campaigns, manage lists, or analyze performance
3. **No coding needed** — natural language commands execute complex API operations
4. **Real-time insights** delivered in formatted responses for quick decision-making

### Who is this for?

Ideal for **marketing teams**, **email marketers**, **growth hackers**, and **agencies** using Zoho Campaign. Let AI agents handle list segmentation, campaign creation, performance analysis, and contact management. Perfect for teams running 10+ campaigns monthly who want to streamline operations, reduce manual tasks, and gain faster insights from campaign data.


## Available Tools
- **add_contacts_to_list**: Each contact requires at minimum an email address. Optionally include first name, last name, phone, company, and custom fields. Contacts must be provided as a JSON array of objects. Returns count of successfully added contacts.

Add contacts to a Zoho Campaign mailing list
- **create_campaign**: Requires campaign name, subject line, sender name, sender email, and reply-to email. Optionally set campaign type, template ID, and scheduling. Returns created campaign details including the new campaign key.

Create a new email campaign in Zoho Campaign
- **create_list**: Requires list name. Optionally set description and welcome message for new subscribers. Returns the created list details including the new list key needed for adding contacts.

Create a new mailing list in Zoho Campaign
- **get_blocked_contacts**: Returns email, reason, and date blocked. Use this to maintain list hygiene and avoid sending to invalid addresses.

List blocked/bounced contacts in Zoho Campaign
- **get_campaign_details**: Use this to review full campaign configuration before sending or editing.

Get details of a specific Zoho Campaign email
- **get_campaign_report**: Includes metrics: total sent, delivered, bounced, opened, clicked, unsubscribed, spam complaints, and forwarded. Also provides engagement breakdown by contact. Use this to analyze campaign ROI and engagement rates.

Get analytics report for a Zoho Campaign
- **get_campaigns**: Returns campaign name, subject line, status, sent date, and basic metrics (sent count, opened, clicked). Use this to review campaign portfolio and performance overview.

List all email campaigns in Zoho Campaign
- **get_contact**: Use this to review individual subscriber details before sending targeted campaigns or troubleshooting delivery issues.

Get details of a specific Zoho Campaign contact
- **get_list_contacts**: Returns contact email, name, subscription status, added date, and custom fields. Use this to review subscriber base, segment audiences, or verify contacts before sending campaigns.

List contacts in a Zoho Campaign mailing list
- **get_lists**: Returns list name, description, contact count, creation date, and status. Mailing lists are used to organize contacts for targeted email campaigns. Use this to review available lists before creating campaigns or adding contacts.

List all mailing lists in Zoho Campaign
- **get_recent_campaigns**: Useful for quick review of latest activity. Type can filter by: all, sent, draft, scheduled. Returns basic campaign info including name, subject, status, and date.

Get recently created or sent campaigns
- **remove_contacts_from_list**: Requires list key and comma-separated email addresses. Use this to manage unsubscribes, clean up lists, or segment contacts. Returns count of successfully removed contacts.

Remove contacts from a Zoho Campaign mailing list
- **update_contact**: Only pass the fields you want to modify. The contact is identified by email address. Returns updated contact data.

Update an existing Zoho Campaign contact


## Installation & Usage

To install and use the **Zoho Campaign** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-campaign](https://vinkius.com/mcp/zoho-campaign)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
