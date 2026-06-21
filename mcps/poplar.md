# Poplar MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/poplar)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/poplar-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/poplar-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Automate programmatic direct mail via Poplar — trigger mailers, standardize addresses, and manage audiences directly from any AI agent.

## Description
Connect your **Poplar** account to any AI agent and take full control of your programmatic direct mail and physical outreach through natural conversation.

### What you can do

- **Trigger Mailers** — Automatically send physical postcards or letters by providing a campaign ID and recipient details.
- **Address Standardization** — Clean and verify US mailing addresses using Poplar's specialized standardization service.
- **Audience Management** — List all mailing audiences and add new members via email or physical address.
- **Suppression Control** — Add recipients to the global 'Do Not Mail' list to manage opt-outs and compliance.
- **Campaign Visibility** — List all active direct mail campaigns and inspect available creatives.
- **Delivery Tracking** — Monitor the production and delivery status of specific mail pieces in real-time.
- **Attribution Reporting** — Submit customer orders back to Poplar to track the ROI of your physical mail campaigns.

### How it works

1. Subscribe to this server
2. Enter your Poplar Access Token (found in API Settings)
3. Start sending physical mail from Claude, Cursor, or any MCP-compatible client

No more manual uploading of address lists. Your AI assistant acts as a dedicated Direct Mail Coordinator or Growth Marketing Specialist.

### Who is this for?

- **Growth Marketers** — automate high-touch physical follow-ups for high-value leads or abandoned carts.
- **Retention Managers** — send 'Win-back' postcards to churning customers directly from the CRM flow.
- **E-commerce Owners** — track the effectiveness of direct mail by reporting transactions back for attribution.


## Available Tools
- **add_to_audience**: Add a recipient to a specific audience list
- **add_to_suppression_list**: Add a recipient to the global "Do Not Mail" list
- **get_api_profile**: Get information about the authenticated account
- **get_mailer_status**: Check the production and delivery status of a specific mailer
- **list_audiences**: List all mailing audiences in your account
- **list_billing_history**: List account billing and invoice data
- **list_marketing_campaigns**: List all direct mail campaigns
- **list_mail_creatives**: List all uploaded mailer designs/creatives
- **standardize_us_address**: Pass fields like address_line1, city, state, postal_code.

Clean and standardize a US mailing address
- **report_transaction**: Report a customer order back to Poplar for attribution tracking
- **trigger_physical_mailer**: Requires "campaign_id" and "recipient_json" (address details). Optional "merge_tags_json" for dynamic content.

Trigger a physical mailer (postcard, letter) for a campaign


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Poplar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a postcard to Jane Doe using campaign ID 'camp_123'."

**🤖 AI Agent:**
> I've started the process for campaign camp_123. To trigger the mailer, I need Jane Doe's full mailing address (street, city, state, zip). Once provided, I'll send the request to Poplar. Should I also include any custom merge tags?

---

**👤 You:**
> "Standardize this address: 123 main st, nyc, ny 10001."

**🤖 AI Agent:**
> Standardizing... Poplar has verified the address. The correct USPS format is: '123 MAIN ST, NEW YORK, NY 10001-4107'. The address is valid and deliverable. Would you like to add this recipient to an audience list?

---

**👤 You:**
> "List all active audiences and find 'Holiday VIPs'."

**🤖 AI Agent:**
> Retrieving audiences... I found 4 groups in your account, including 'Holiday VIPs' (ID: aud_552) with 1,200 members. Other audiences are 'New Signups', 'Churn Risks', and 'Global Suppressions'. Should I list the members of 'Holiday VIPs'?


## Installation & Usage

To install and use the **Poplar** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/poplar](https://vinkius.com/mcp/poplar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
