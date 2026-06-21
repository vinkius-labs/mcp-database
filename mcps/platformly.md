# Platform.ly MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/platformly)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/platformly-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/platformly-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Grow your business with marketing automation, CRM, and analytics connected in one platform that shows what drives revenue.

## Description
Connect your **Platform.ly** account to any AI agent and take full control of your business automation and CRM orchestration through natural conversation. Platform.ly is a powerful multi-channel marketing platform, and this integration allows you to retrieve contact metadata, manage sales pipelines, and trigger automated events directly from your chat interface.

### What you can do

- **Contact & CRM Orchestration** — List, add, and update contacts with detailed profile metadata programmatically to ensure your audience database is always synchronized.
- **Sales Pipeline Intelligence** — Access and monitor your sales pipelines and create new deals directly from the AI interface to track revenue growth and deal velocity.
- **Tag & Segment Control** — Apply or remove tags and manage segments via natural language to drive better targeted marketing efficiency.
- **Automation & Event Management** — Fire custom events and add notes to contacts to ensure your automated workflows are always synchronized.
- **Operational Monitoring** — Track system status and manage organization metadata using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your Platform.ly API Key from your account settings
3. Start managing your CRM and automation from Claude, Cursor, or any MCP-compatible client

No more manual data entry or missed follow-ups. Your AI acts as a dedicated marketing operations manager or sales coordinator.

### Who is this for?

- **Marketing Automation Experts** — quickly retrieve segment summaries and monitor campaign performance without switching apps.
- **Sales Teams** — automate the management of deal pipelines and track lead engagement via natural conversation.
- **Business Owners** — streamline the retrieval of contact metadata and monitor organizational health directly within the chat.


## Available Tools
- **create_new_contact**: Requires project ID and email.

Add a new contact to the CRM
- **add_note_to_contact**: Add a text note to a contact
- **apply_tag_to_contact**: Add a tag to a contact
- **create_new_sales_deal**: Create a new deal in a pipeline
- **get_contact_details**: Get full info for a contact
- **list_crm_contacts**: List contacts in a project
- **list_sales_pipelines**: List all sales pipelines
- **list_project_segments**: List all segments in a project
- **list_project_tags**: List all tags in a project
- **remove_tag_from_contact**: Remove a tag from a contact
- **search_contact_by_email**: Find a contact by email
- **update_existing_contact**: Modify a contact record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Platform.ly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active contacts in project ID 1234."

**🤖 AI Agent:**
> I've retrieved your contacts for project 1234. You have 50 active profiles. Notable recent additions include 'Alice Miller' and 'Sarah Chen'. Which one would you like to see pipeline details for?

---

**👤 You:**
> "Show me the performance of my active email automation sequences and their conversion funnels."

**🤖 AI Agent:**
> You have 5 active automation sequences. "Welcome Series" (4 emails) has 68% open rate and 12% click-through, converting 340 of 2,800 new subscribers to trial users. "Re-engagement Campaign" recovered 89 inactive users this month (15% reactivation rate). "Upgrade Nudge" drives $4,200/mo in upsells with 8% conversion. "Onboarding Drip" has the highest completion rate at 74%. Total automation-driven revenue this month: $18,400.

---

**👤 You:**
> "Create a new contact segment for users who signed up in the last 14 days but have not completed onboarding."

**🤖 AI Agent:**
> Segment created: "New Users - Onboarding Incomplete" (ID: seg_4821). Matching contacts: 127 users. Criteria: signup date within 14 days AND onboarding_completed equals false. Demographics: 62% from organic search, 24% from paid ads, 14% from referrals. Average time since signup: 8.3 days. This segment is now available for targeting in automation sequences and broadcast campaigns.


## Installation & Usage

To install and use the **Platform.ly** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/platformly](https://vinkius.com/mcp/platformly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
