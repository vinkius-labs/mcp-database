# ChatBot.com MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chatbotcom)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/chatbotcom-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/chatbotcom-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage conversational AI and bot workflows via ChatBot — track stories, interactions, and user data directly from any AI agent.

## Description
Connect your **ChatBot.com** account to any AI agent and take full control of your conversational automation through natural conversation. Streamline how you build and monitor your customer service bots.

### What you can do

- **Story Oversight** — List and retrieve details for all conversational stories and bot workflows natively
- **Interaction Intelligence** — Access and monitor interactions within specific stories to understand user paths flawlessly
- **User Management** — List all users who have interacted with your bot and retrieve their detailed profiles securely
- **Integration Auditing** — List and review configured webhook integrations and entities flawlessly
- **Training Logistics** — Retrieve unrecognized phrases to identify areas where your bot needs additional training flawlessly
- **System Metadata** — Access entity definitions and core account structures directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your ChatBot Developer Access Token (obtained from your settings)
3. Start managing your conversational AI from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Customer Experience Managers** — monitor bot performance and review user interactions using natural language
- **Conversational Designers** — audit stories and interactions without opening the complex dashboard
- **Support Teams** — quickly look up user details and chat histories straight from their chat interface
- **Product Managers** — identify bot training needs and analyze entity usage for roadmap planning


## Available Tools
- **get_story_details**: Get detailed information for a specific story
- **get_chatbot_user_details**: Get details for a specific chatbot user
- **list_chatbot_entities**: List custom entities used for NLP matching
- **list_story_interactions**: List all interactions within a story
- **list_chatbot_stories**: List all stories (bot workflows)
- **list_training_data**: List unrecognized phrases that require bot training
- **list_chatbot_users**: List all users who have interacted with the bot
- **list_chatbot_webhooks**: List all configured webhook integrations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ChatBot.com** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all conversational stories in my account."

**🤖 AI Agent:**
> Retrieving your stories... I found 4 items: 'Main Greeting', 'Product FAQ', 'Lead Generation', and 'Customer Support Flow'. Which one would you like to see details for?

---

**👤 You:**
> "What training data is pending review?"

**🤖 AI Agent:**
> Checking for unrecognized phrases... I found 15 phrases that users typed but the bot didn't recognize, such as 'How do I cancel?' and 'Talk to human'.

---

**👤 You:**
> "Search for users who interacted with the bot today."

**🤖 AI Agent:**
> Retrieving today's users... I found 25 unique users who interacted with the bot. 10 provided an email address during their session.


## Installation & Usage

To install and use the **ChatBot.com** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chatbotcom](https://vinkius.com/mcp/chatbotcom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
