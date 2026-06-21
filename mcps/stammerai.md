# Stammer.ai MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stammerai)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/stammerai-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/stammerai-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage white-label AI chatbots, knowledge bases, and sub-accounts on Stammer.ai with AI agents.

## Description
Connect your **Stammer.ai** account to any AI agent to automate your white-label AI agency and chatbot orchestration. Stammer.ai provides a premier platform for agencies to build and resell custom AI agents, and this integration allows you to retrieve chatbot metadata, manage knowledge bases, and track sub-account performance through natural conversation.

### What you can do

- **Chatbot Orchestration** — List all managed chatbots and retrieve detailed profile metadata, including status and configuration programmatically.
- **Knowledge Base Lifecycle Management** — Add new Q&A pairs and website URLs to your chatbots' knowledge base directly from the AI interface to ensure they are always informed.
- **Sub-Account & User Control** — Access and monitor your agency's sub-accounts and user database to maintain a clear overview of your resell operations.
- **Message & Interaction Tracking** — Retrieve recent chat messages and monitor conversational logs via natural language commands to ensure high-quality interactions.
- **Operational Monitoring** — Check system health and manage agency metadata to ensure your white-label platform is always optimized.

### How it works

1. Subscribe to this server
2. Enter your Stammer.ai API Key from your agency dashboard
3. Start managing your AI agency from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Agency Owners** — quickly retrieve sub-account details and monitor chatbot performance without switching tabs.
- **AI Developers** — automate the process of updating knowledge bases and testing chatbot responses via natural conversation.
- **Customer Success Teams** — streamline the retrieval of conversational logs and monitor user engagement directly within the chat.


## Available Tools
- **add_qa**: Add a Q&A pair to knowledge base
- **add_url**: Add a URL to scrape for knowledge base
- **create_chatbot**: Create a new AI chatbot
- **get_chatbot**: Get details for a specific chatbot
- **get_knowledge_base**: Get the knowledge base for a chatbot
- **get_sub_account**: Get details for a sub-account
- **list_chatbots**: ai account.

List all AI agents (chatbots)
- **list_knowledge_base**: List knowledge base items for a chatbot
- **list_messages**: List chat messages for a chatbot
- **list_sub_accounts**: List all white-label sub-accounts
- **list_users**: List all users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stammer.ai** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active chatbots in my Stammer.ai account."

**🤖 AI Agent:**
> I've retrieved your chatbots. You have 3 active bots online: 'Customer Support Lead', 'Real Estate Assistant', and 'Onboarding Specialist'. Which one would you like to update?

---

**👤 You:**
> "Show me the performance analytics for all deployed AI chatbots with conversation metrics."

**🤖 AI Agent:**
> 5 deployed chatbots. "Sales Assistant" (GPT-4): 1,234 conversations this month, 78% resolution rate, avg 4.2 messages per conversation, lead capture rate 34%. "Support Bot" (GPT-4): 2,890 conversations, 85% resolution, avg 6.1 messages, ticket reduction 45%. "FAQ Helper" (GPT-3.5): 4,560 conversations, 92% accuracy, avg 2.3 messages. "Onboarding Guide" (GPT-4): 567 conversations, 89% completion. "Internal HR" (GPT-4): 345 conversations, 91% satisfaction. Total tokens used: 12.4M. Monthly cost: $234.

---

**👤 You:**
> "Add 20 new FAQ entries to the Support Bot knowledge base from our latest help center articles."

**🤖 AI Agent:**
> 20 FAQ entries added to Support Bot knowledge base. Categories: Billing (5 entries), Account Management (4), Technical Setup (4), Integrations (3), Security (2), API Usage (2). Source: Help Center articles published May 1-15. Training status: complete (re-indexed in 12 seconds). Knowledge base size: 234 entries → 254 entries. Confidence threshold: maintained at 85%. Test results: 18/20 new entries correctly matched to test queries (90% accuracy). 2 entries flagged for review (ambiguous intent overlap with existing entries).


## Installation & Usage

To install and use the **Stammer.ai** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stammerai](https://vinkius.com/mcp/stammerai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
