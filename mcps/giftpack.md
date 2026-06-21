# Giftpack MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/giftpack)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/giftpack-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/giftpack-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Manage AI-curated corporate gifting, track campaigns, and oversee recipients via AI agents with Giftpack AI.

## Description
Connect your **Giftpack** account to any AI agent to automate your corporate gifting and employee recognition workflows through the Model Context Protocol (MCP). Giftpack AI uses advanced algorithms to curate the perfect gifts for your recipients based on their preferences and milestones. This MCP server enables you to manage your recipient database (members), create AI-powered gifting campaigns (orders), and track the entire gifting lifecycle directly through natural conversation.

### Key Features

- **Recipient Management** — List all members in your workspace, retrieve detailed profile metadata, and programmatically add new recipients (employees, clients, or friends).
- **AI Order Orchestration** — Create new AI gifting campaigns with specific budgets and recipients, and retrieve detailed configuration metadata for each order.
- **Launch Automation** — Formally launch gifting campaigns once budgets are verified directly from your chat interface.
- **Gift Discovery** — Retrieve the list of AI-curated gift options for any specific receiver to understand what's being offered.
- **Milestone Tracking** — List available gifting purposes (onboarding, anniversaries, birthdays) to align your campaigns with business events.
- **Workspace Oversight** — Access metadata for your authenticated workspace to verify connectivity and authorized scopes.
- **Real-time Synchronization** — Keep your relationship-driven gifting data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Giftpack Workspace ID and API Key (found in Integration Hub)
3. Start managing your corporate gifting from Claude, Cursor, or any MCP client

### Who is this for?

- **HR & Ops Managers** — quickly check if an employee's onboarding gift has been curated or launch a birthday campaign without manual dashboard navigation.
- **Customer Success Leads** — automate the management of client appreciation gifts via simple AI commands.
- **Executive Assistants** — get a real-time overview of active gifting campaigns and recipient statuses.


## Available Tools
- **verify_api_connection**: Check connection
- **create_gifting_campaign**: Start AI order
- **create_gifting_member**: Add new recipient
- **get_gifting_campaign_details**: Get order metadata
- **get_member_details**: Get recipient metadata
- **list_curated_gift_options**: List AI gifts
- **launch_gifting_campaign**: Activate AI order
- **list_gifting_campaigns**: List AI orders
- **list_gifting_milestones**: g. onboarding, birthday).

List gifting purposes
- **list_gifting_members**: List all recipients
- **list_campaign_receivers**: List order recipients
- **modify_gifting_campaign**: Update AI order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Giftpack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active members in my Giftpack workspace."

**🤖 AI Agent:**
> Retrieving members... I found 5 active recipients, including 'Jane Doe' (Employee) and 'Acme Corp' (Client). Would you like to see the profile details for any of them?

---

**👤 You:**
> "Check the status of AI Order 'ord_12345'."

**🤖 AI Agent:**
> Fetching order... AI Order ord_12345 is currently in 'Draft' status with a budget of $500. It has 10 recipients assigned. Would you like to launch it?

---

**👤 You:**
> "Create a new gifting campaign for 'Holiday Rewards' with a $1000 budget."

**🤖 AI Agent:**
> Campaign created! I've successfully set up the 'Holiday Rewards' AI order with a budget of $1000 USD. You can now add recipients and launch the campaign.


## Installation & Usage

To install and use the **Giftpack** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/giftpack](https://vinkius.com/mcp/giftpack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
