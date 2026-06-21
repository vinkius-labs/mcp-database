# MRPLN MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mrpln)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mrpln-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mrpln-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Plan manufacturing resources with production scheduling, material requirements, and capacity planning for growing factories.

## Description
Connect your **MRPLN** account to any AI agent to streamline your marketing automation and multi-channel customer engagement. MRPLN provides a unified platform for WhatsApp, SMS, and Email automation powered by AI.

### What you can do

- **Customer Management** — Create, update, and list customers to maintain a clean and actionable marketing database
- **WhatsApp Business API** — Access your approved WABA templates and send highly engaging messages directly through Meta's official API
- **Multi-channel Messaging** — Send immediate or automated messages via SMS and Email to reach your audience where they are
- **Tactic Monitoring** — List and retrieve performance analytics for your marketing tactics to optimize ROI in real-time
- **Template Management** — List and use pre-approved message templates for consistent brand communication

### How it works

1. Subscribe to this server
2. Enter your MRPLN API Key from your dashboard settings
3. Start managing your marketing planning and execution from Claude, Cursor, or any MCP client

### Who is this for?

- **Marketing Agencies** — manage multiple customer flows and multi-channel campaigns efficiently
- **E-commerce Owners** — automate post-purchase engagement and recovery via WhatsApp and SMS
- **Sales Teams** — qualify leads and maintain high-touch engagement across different channels


## Available Tools
- **create_customer**: Create a new customer/lead
- **get_customer**: Get details for a specific customer
- **get_tactic_performance**: Get performance analytics for a tactic
- **list_customers**: List all customers/leads
- **list_tactics**: List all marketing tactics
- **list_waba_templates**: List WhatsApp Business templates
- **send_email_message**: Send an email
- **send_sms_message**: Send an SMS message
- **send_whatsapp_message**: Pass components as a JSON string.

Send a WhatsApp message
- **update_customer**: Update an existing customer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MRPLN** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all customers in my MRPLN account."

**🤖 AI Agent:**
> I've retrieved your customer list. You have 45 registered leads, including 'John Smith' and 'Maria Garcia'. Would you like to see the details for a specific customer?

---

**👤 You:**
> "Send a WhatsApp message to +123456789 using the 'welcome_template'."

**🤖 AI Agent:**
> WhatsApp message sent successfully to +123456789! I used the 'welcome_template' as requested.

---

**👤 You:**
> "Show me the performance of the 'Winter Sale' tactic."

**🤖 AI Agent:**
> The 'Winter Sale' tactic has achieved a 15% conversion rate so far, with 200 messages sent and 30 conversions recorded. Would you like to see a channel breakdown?


## Installation & Usage

To install and use the **MRPLN** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mrpln](https://vinkius.com/mcp/mrpln)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
