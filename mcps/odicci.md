# Odicci MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/odicci)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/odicci-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/odicci-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Launch interactive marketing campaigns with gamification elements like spin wheels, quizzes, and scratch cards that capture leads.

## Description
Connect your **Odicci** account to any AI agent and take full control of your interactive marketing orchestration and gamification through natural conversation. Odicci provides a premier platform for creating engaging customer experiences like quizzes, polls, and instant-win games, and this integration allows you to retrieve experience metadata, manage customer profiles, and monitor campaign segments directly from your chat interface.

### What you can do

- **Experience & Campaign Orchestration** — List all managed interactive experiences and retrieve detailed configuration metadata programmatically to ensure your marketing loops are always synchronized.
- **Customer Lifecycle Management** — Access and monitor your centralized customer database and create or update profiles directly from the AI interface to maintain a high-fidelity CRM.
- **Segment & Audience Control** — Access and monitor audience segments via natural language to drive better targeted engagement and campaign personalization.
- **Reward & Prize Oversight** — Access and monitor prize distributions and reward metadata to ensure your gamification strategy is always optimized using simple AI commands.
- **Operational Monitoring** — Track system responses and manage customer interactions to ensure your interactive workflows are always high-performing.

### How it works

1. Subscribe to this server
2. Enter your Odicci Secret API Key from your account settings
3. Start managing your interactive marketing from Claude, Cursor, or any MCP-compatible client

No more manual exporting of participant data for simple checks. Your AI acts as a dedicated engagement coordinator or campaign analyst.

### Who is this for?

- **Marketing Managers** — quickly retrieve campaign summaries and monitor participation rates without switching apps.
- **CRM Specialists** — automate the management of customer records and track segment growth via natural conversation.
- **Developers** — integrate real-time interactive marketing data and customer profiles directly within the chat.


## Available Tools
- **check_odicci_status**: Verify connectivity
- **create_customer**: Create a customer
- **create_experience**: Create an experience
- **get_customer**: Get customer details
- **get_experience_stats**: Get experience stats
- **get_experience**: Get experience details
- **get_segment**: Get segment details
- **list_customers**: List customers
- **list_experiences**: List experiences
- **list_rewards**: List rewards
- **list_segments**: List segments
- **search_customers**: Search customers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Odicci** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active interactive experiences in Odicci."

**🤖 AI Agent:**
> I've retrieved your experiences. You have 3 active campaigns including 'Summer Quiz' and 'Instant Win Wheel'. Which one would you like to see customer entries for?

---

**👤 You:**
> "Show me the engagement statistics for my Summer Giveaway experience."

**🤖 AI Agent:**
> Your Summer Giveaway experience (ID: exp_3421) has generated 2,847 total interactions over 14 days. Unique participants: 1,923. Completion rate: 68%. Email opt-ins collected: 1,308 (68% of participants). Top traffic source: Instagram Stories (42%), followed by email campaigns (31%) and website embed (27%).

---

**👤 You:**
> "Search for all customers who participated in experiences tagged with loyalty."

**🤖 AI Agent:**
> I found 456 customers who engaged with loyalty-tagged experiences. Top segment: "Repeat Buyers" with 203 customers (45%). Average interactions per customer: 3.2. Most active customer: Sarah Martinez with 12 completed experiences. 78% of these customers have opted in for email communications.


## Installation & Usage

To install and use the **Odicci** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/odicci](https://vinkius.com/mcp/odicci)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
