# Zendesk QA (Klaus) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zendesk-qa-klaus)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zendesk-qa-klaus-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zendesk-qa-klaus-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Export QA reviews, search conversations, and import ticket data via the Klaus (Zendesk QA) API.

## Description
Connect your **Zendesk QA** (formerly Klaus) account to any AI agent to automate your customer service quality assurance workflows. This MCP server enables your agent to export quality scores, search for reviewed conversations, and import external ticket data directly from natural language interfaces.

### What you can do

- **Review Extraction** — List all quality assurance reviews and internal quality scores (IQS) account-wide or by workspace
- **Workspace Management** — List all available workspaces to organize your QA processes and review assignments
- **Conversation Discovery** — Search for specific customer interactions to identify which ones have been graded
- **Data Integration** — Import conversation data and agent profiles from external platforms for grading in Zendesk QA
- **Record Maintenance** — Permanently remove ticket data from the QA platform via simple commands

### How it works

1. Subscribe to this server
2. Enter your Zendesk Subdomain and QA API Token
3. Start managing your support quality from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Managers** — Monitor support quality trends and export review data for reporting via natural language
- **Support Leads** — Quickly search for agent reviews and identify areas for improvement from your dev tools
- **Operations Teams** — Automate the synchronization of external ticket data into the QA platform effortlessly


## Available Tools
- **delete_qa_tickets**: Remove specific ticket data from the QA platform
- **import_qa_tickets**: Import conversation data into Zendesk QA for review
- **import_qa_users**: Sync agents and managers into Zendesk QA
- **list_all_reviews**: List all quality assurance reviews account-wide
- **search_qa_conversations**: Search for conversations in Zendesk QA
- **list_workspace_reviews**: List reviews for a specific workspace
- **list_qa_workspaces**: Use this to identify workspace IDs for exporting reviews.

List all Zendesk QA workspaces


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zendesk QA (Klaus)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Zendesk QA workspaces."

**🤖 AI Agent:**
> I've retrieved your workspaces. You have 3 active environments: 'English Support', 'Spanish Support', and 'Technical Escalations'. Which one would you like to access?

---

**👤 You:**
> "Show recent QA reviews for the 'English Support' workspace (ID: '123')."

**🤖 AI Agent:**
> I found 10 recent reviews for the English Support workspace. The average Internal Quality Score (IQS) is 92%. Notable recent reviews include tickets #ORD-987 and #TECH-101.

---

**👤 You:**
> "Search for reviewed conversations associated with client email 'user@example.com'."

**🤖 AI Agent:**
> I've searched your account and found 2 conversations for 'user@example.com' that have been graded. Ticket #12345 received a score of 100% and Ticket #12346 received a score of 85%.


## Installation & Usage

To install and use the **Zendesk QA (Klaus)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zendesk-qa-klaus](https://vinkius.com/mcp/zendesk-qa-klaus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
