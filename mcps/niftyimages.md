# NiftyImages MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/niftyimages)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/niftyimages-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/niftyimages-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage personalized images and dynamic content via NiftyImages — track images, widgets, and countdown timers directly from your AI agent.

## Description
Connect your **NiftyImages** account to your AI agent and take control of your dynamic email and web content through natural conversation.

### What you can do

- **Asset Management** — List all personalized images and dynamic widgets available in your account.
- **Performance Tracking** — Retrieve aggregated impression and click statistics for images and widgets to monitor engagement.
- **Timer Control** — Dynamically update the target end date and time for your active countdown timers.
- **Data Store Operations** — List fields, add new personalization records, and manage your custom data stores.
- **Photoshop Integration** — Programmatically update specific layers in your Photoshop-designed dynamic images.
- **Deep Inspection** — Fetch complete metadata and configuration for specific assets using their Image Keys.

### How it works

1. Subscribe to this server
2. Enter your NiftyImages API Key
3. Start managing your dynamic content from Claude, Cursor, or any MCP client

### Who is this for?

- **Email Marketers** — quickly check asset performance or update timer deadlines without opening the NiftyImages portal.
- **Creative Operations** — automate the update of personalization data and image layers directly from your workspace.
- **Marketing Analysts** — retrieve real-time engagement metrics for dynamic content reporting.


## Available Tools
- **add_datastore_record**: Add record to data store
- **delete_datastore_record**: Delete record from data store
- **get_image_stats**: Get image performance stats
- **get_image**: Get specific image details
- **get_widget_stats**: Get widget performance stats
- **list_datastore_fields**: List fields for a data store
- **list_images**: List all NiftyImages
- **list_widgets**: ) created in your account.

List all dynamic widgets
- **update_psd_image**: Update Photoshop layers
- **update_timer**: Update countdown timer date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NiftyImages** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all the personalized images in my NiftyImages account."

**🤖 AI Agent:**
> Retrieving your images... I found 12 personalized images, including 'Welcome Banner' (Key: img_123), 'Abandoned Cart Promo', and 'Birthday Surprise'. Would you like the performance stats for the Welcome Banner?

---

**👤 You:**
> "Update the countdown timer 'SaleEnd' to expire on December 25th, 2024 at midnight."

**🤖 AI Agent:**
> Target date update initiated... The timer 'SaleEnd' (Key: timer_987) has been successfully updated. It is now set to expire on 2024-12-25 00:00:00. All users opening the email from now on will see the new deadline.

---

**👤 You:**
> "Show me the impression and click stats for all my images."

**🤖 AI Agent:**
> Fetching image statistics... Your assets have generated a total of 1.2M impressions and 45K clicks this month. The 'Promo Banner' is your top performer with a 5.2% click-through rate. Shall I provide the breakdown for the dynamic widgets as well?


## Installation & Usage

To install and use the **NiftyImages** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/niftyimages](https://vinkius.com/mcp/niftyimages)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
