# CoderPad MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coderpad)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/coderpad-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/coderpad-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage technical interviews and assessments via CoderPad — create pads, track interview events, and audit the question bank directly from any AI agent.

## Description
Connect your **CoderPad** account to any AI agent and take full control of your technical hiring process through natural conversation. Streamline how you prepare, conduct, and review technical interviews natively.

### What you can do

- **Pad Management** — Create and list live collaborative coding pads for technical interviews natively
- **Session Intelligence** — Access detailed information for specific pads, including the current code contents and status flawlessly
- **Event Tracking** — Retrieve a play-by-play log of all actions within an interview session, including typing and execution flawlessly
- **Question Logistics** — List and review available interview questions from your organization's question bank securely
- **Team Management** — List all users and interviewers within your organization to manage access flawlessly
- **integrated Visibility** — Retrieve detailed pad metadata including titles, languages, and candidate names directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your CoderPad API Key (found in Settings > API)
3. Start managing your technical interviews from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Technical Recruiters** — automate pad creation and verify candidate progress using natural language
- **Hiring Managers** — audit interview event logs and review code submissions without opening the dashboard
- **Software Engineers** — quickly prepare interview environments and look up questions straight from their chat interface
- **Ops Teams** — verify account usage history and monitor interviewer roles


## Available Tools
- **create_new_interview_pad**: Create a new live collaborative coding pad
- **get_my_coderpad_profile**: Retrieve information about the authenticated user
- **get_pad_event_log**: Retrieve a play-by-play log of all actions in a specific pad
- **get_pad_session_details**: Get detailed information for a specific pad, including current code contents
- **list_coderpad_org_users**: List all users and interviewers in the organization account
- **list_coderpad_sessions**: List all technical interview pads (sessions)
- **list_coderpad_questions**: List available interview questions from the question bank
- **get_coderpad_usage_history**: Retrieve a history of pad usage and quota consumption


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CoderPad** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my CoderPad sessions from this week."

**🤖 AI Agent:**
> Retrieving your recent sessions... I found 5 pads: 'Backend Dev - John Doe', 'Frontend Role - Sarah Smith', and 3 others. 2 are still 'Live' and 3 are 'Completed'. Would you like the code for any of these?

---

**👤 You:**
> "Create a new Python pad for 'Junior Engineer Interview'."

**🤖 AI Agent:**
> Creating Python pad... The session has been successfully created. You can invite the candidate using this URL: [Pad URL]. I can also preload a question if you'd like.

---

**👤 You:**
> "Show me the last 5 questions in my question bank."

**🤖 AI Agent:**
> Retrieving questions... The 5 newest questions are: 'System Design: URL Shortener', 'Binary Tree Traversal', 'SQL: Top Customers', 'React: Todo List', and 'Python: Palindrome Check'.


## Installation & Usage

To install and use the **CoderPad** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coderpad](https://vinkius.com/mcp/coderpad)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
