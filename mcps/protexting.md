# ProTexting MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/protexting)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/protexting-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/protexting-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate SMS marketing via ProTexting — manage campaigns, contacts, and keywords directly with AI.

## Description
Connect your **ProTexting** account to any AI agent and take full control of your business text messaging and SMS orchestration through natural conversation. ProTexting provides a premier platform for mobile marketing and customer engagement, and this integration allows you to send SMS/MMS, manage contact groups, and monitor keyword performance directly from your chat interface.

### What you can do

- **SMS & Messaging Orchestration** — Send individual or bulk text messages programmatically to ensure your outreach is always synchronized.
- **Contact & Group Management** — Create and organize mobile contacts into segments and groups directly from the AI interface to maintain a high-fidelity audience.
- **Keyword & Campaign Intelligence** — Access and monitor mobile keywords and campaign stats via natural language to drive better engagement.
- **Inbox & Conversation Control** — Access your mobile inbox and retrieve real-time message metadata to ensure rapid customer responses.
- **Operational Monitoring** — Track account stats and manage system metadata using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your ProTexting OAuth Access Token from your developer settings
3. Start managing your SMS marketing from Claude, Cursor, or any MCP-compatible client

No more manual typing or spreadsheet contact updates. Your AI acts as a dedicated mobile marketing coordinator or customer success coordiator.

### Who is this for?

- **Marketing Managers** — quickly send promotional SMS and monitor keyword performance without switching apps.
- **Customer Support Teams** — automate the retrieval of incoming messages and respond to clients via natural conversation.
- **Operations Teams** — streamline the retrieval of contact metadata and monitor organizational SMS health directly within the chat.


## Available Tools
- **check_protexting_status**: Verify connectivity
- **create_contact**: Create a contact
- **create_group**: Create a group
- **delete_contact**: Delete a contact
- **get_account**: Get account info
- **get_message_status**: Get message status
- **list_contacts**: List contacts
- **list_groups**: List groups
- **list_keywords**: List keywords
- **send_bulk**: Send bulk messages
- **send_mms**: Send MMS
- **send_sms**: Send SMS


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ProTexting** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my contact groups in ProTexting."

**🤖 AI Agent:**
> I've retrieved your groups. You have 3 active segments: 'VIP Customers', 'New Leads', and 'Event Attendees'. Which one would you like to send a message to?

---

**👤 You:**
> "Show me all active text messaging campaigns and their opt-in subscriber counts."

**🤖 AI Agent:**
> 6 active campaigns. "Loyalty Rewards" has 4,234 opt-in subscribers (grew 12% this month), 89% delivery rate, 34% redemption rate on offers. "Weekly Specials" reaches 3,891 subscribers with 92% delivery. "Appointment Reminders" serves 2,456 contacts with 97% delivery and reduced no-shows by 42%. "Flash Sales" has 1,678 subscribers. "Birthday Club" has 890 members. "Event Alerts" has 567. Total active subscribers: 13,716.

---

**👤 You:**
> "Send a promotional text blast to all Loyalty Rewards subscribers with a 20% discount code."

**🤖 AI Agent:**
> Promotional text blast sent to 4,234 Loyalty Rewards subscribers. Message: "Exclusive for you! Save 20% on your next visit with code LOYAL20. Valid through May 31st. Show this text at checkout. Reply STOP to opt out." Delivery: 4,189 delivered (98.9%), 45 undeliverable. Compliance: TCPA compliant with opt-out included. Based on previous promotions, expect 340-420 redemptions (8-10% conversion) generating approximately $6,800 in revenue.


## Installation & Usage

To install and use the **ProTexting** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/protexting](https://vinkius.com/mcp/protexting)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
