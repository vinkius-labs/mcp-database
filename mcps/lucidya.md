# Lucidya MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lucidya)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/lucidya-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/lucidya-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Monitor social media, analyze sentiment, and manage customer data via the Lucidya API.

## Description
Connect your **Lucidya** account to any AI agent to automate your social listening and customer engineering intelligence. This MCP server enables your agent to list monitors, analyze text sentiment using advanced AI, and retrieve unified customer profiles directly from natural language interfaces.

### What you can do

- **Social Listening** — List all active and inactive monitors across Twitter, Instagram, and other sources
- **AI Analysis** — Perform advanced sentiment analysis and Arabic dialect detection on any text string
- **CDP Access** — Retrieve unified customer profiles and interaction histories from the Lucidya Customer Data Platform
- **Service Analytics** — Query KPIs and performance metrics for customer service via the OmniServe API
- **Real-time Monitoring** — Fetch complete metadata and status for your configured listening monitors

### How it works

1. Subscribe to this server
2. Enter your Lucidya API Token
3. Start managing your social intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Brand Managers** — Monitor social mentions and brand sentiment via simple natural language commands
- **Customer Experience Teams** — Quickly retrieve unified customer profiles and interaction histories
- **Data Analysts** — Automate the extraction of social metrics and AI-driven sentiment logs into your workflow


## Available Tools
- **get_omniserve_analytics**: Query customer service analytics KPIs
- **list_cdp_customers**: List customer profiles from CDP
- **detect_arabic_dialect**: Detect the specific Arabic dialect of a text
- **get_customer_profile**: Get complete details for a customer profile
- **get_monitor_details**: Get details for a specific monitor
- **list_social_monitors**: List all social media monitors
- **analyze_text_sentiment**: Analyze the sentiment of a given text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lucidya** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my social media monitors in Lucidya."

**🤖 AI Agent:**
> I've retrieved your monitors. You have 5 active monitors, including 'Competitor Tracking', 'Brand Mentions', and 'Campaign Launch 2024'.

---

**👤 You:**
> "Analyze the sentiment of this text: 'I am extremely happy with the new product release!'."

**🤖 AI Agent:**
> The AI analysis confirms a 🟢 Positive sentiment for that text, with a high confidence score of 0.98.

---

**👤 You:**
> "Show the customer profile for ID 'cust-123' in the Lucidya CDP."

**🤖 AI Agent:**
> I've fetched the profile for customer cust-123. They have interact with your brand 12 times across Twitter and Intercom, with an overall sentiment score of 0.85 (Neutral-Positive).


## Installation & Usage

To install and use the **Lucidya** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lucidya](https://vinkius.com/mcp/lucidya)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
