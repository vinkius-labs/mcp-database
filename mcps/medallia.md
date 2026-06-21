# Medallia MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/medallia)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/medallia-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/medallia-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Customer experience management via Medallia — track surveys, responses, and experience programs.

## Description
Connect your **Medallia** experience management instance to any AI agent and take full control of your customer feedback and CX programs through natural conversation.

### What you can do

- **Survey Management** — List all customer surveys and fetch detailed configuration metadata
- **Feedback Monitoring** — Retrieve and search survey responses to understand customer sentiment in real-time
- **Program Oversight** — List and inspect experience management programs and their statuses
- **Alert Management** — Monitor and retrieve details for alerts triggered by specific customer feedback
- **User Inventory** — List authorized users and manage access within your Medallia instance

### How it works

1. Subscribe to this server
2. Enter your Medallia Base URL, Client ID, and Client Secret
3. Start managing your CX intelligence from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_alert**: Get details for a specific alert
- **get_program_details**: Get details for a specific program
- **get_response**: Get details for a specific response
- **get_survey**: Get details for a specific survey
- **list_alerts**: List feedback alerts
- **list_programs**: List experience management programs
- **list_responses**: List survey responses
- **list_surveys**: List all customer surveys
- **list_users**: List Medallia users
- **search_responses**: Search survey responses by term


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Medallia** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active surveys in Medallia."

**🤖 AI Agent:**
> Retrieving surveys... I found several active surveys including 'Post-Purchase Feedback' and 'Customer Satisfaction 2024'.

---

**👤 You:**
> "Search responses for the term 'disappointed'."

**🤖 AI Agent:**
> Searching... I identified 5 responses containing the term 'disappointed'. Would you like to see the details for these entries?

---

**👤 You:**
> "Show recent alerts from high-priority programs."

**🤖 AI Agent:**
> Querying alerts... There are 3 new alerts triggered by low NPS scores in the 'Premium Support' program.


## Installation & Usage

To install and use the **Medallia** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/medallia](https://vinkius.com/mcp/medallia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
