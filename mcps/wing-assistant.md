# Wing Assistant MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wing-assistant)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wing-assistant-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wing-assistant-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your Wing virtual assistants and delegate tasks programmatically through AI.

## Description
Connect your **Wing Assistant** account to any AI agent to automate your delegation workflows and manage your virtual team. Wing provides a managed service that combines AI efficiency with human expertise, and this integration allows you to interact with your assistants through natural conversation.

### What you can do

- **Assistant Orchestration** — List all your active virtual assistants and retrieve detailed metadata about their roles and skills.
- **Task Delegation** — Delegate new units of work by creating tasks directly in your assistant's queue with clear instructions and priorities.
- **Real-time Lifecycle Control** — Update task details, instructions, and statuses programmatically to ensure project alignment.
- **Operational Monitoring** — Track task progress and history across your entire workspace to stay updated on your virtual team's output.
- **Resource Navigation** — Monitor your assistant's current workload and capacity to optimize your delegation strategy.

### How it works

1. Subscribe to this server
2. Enter your Wing Assistant API Access Token (Bearer) from your dashboard
3. Start delegating tasks to your virtual team from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Executives & Founders** — quickly delegate administrative or research tasks via natural conversation without switching apps.
- **Operations Managers** — automate the flow of work to virtual assistants and monitor progress in real-time.
- **Growth Teams** — scale your operations by programmatically managing tasks for specialized virtual talent.


## Available Tools
- **create_task**: Provide title and description.

Create a new task for an assistant
- **get_assistant**: Get details of a specific assistant
- **get_task_status**: Get current status of a unit of work
- **list_assistants**: List all active virtual assistants
- **list_tasks**: List all tasks assigned to assistants
- **update_task**: Update an existing task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wing Assistant** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new task for my virtual team to 'Compile a list of 50 local real estate agencies in Miami' and include detailed instructions to find their contact emails."

**🤖 AI Agent:**
> I have successfully created the task 'Compile a list of 50 local real estate agencies in Miami' and added your instructions. It has been assigned to your active General Admin assistant and is currently in the 'pending' queue.

---

**👤 You:**
> "Check the status of task ID 'TSK-8492' and if it's still pending, update the priority instructions to 'Urgent - Need by EOD today'."

**🤖 AI Agent:**
> I checked task 'TSK-8492' and it was still marked as pending. I have updated the instructions with your urgent priority note. Your assistant will be notified of this change immediately.

---

**👤 You:**
> "Show me the current workload and active tasks assigned to my assistant 'Maria'."

**🤖 AI Agent:**
> I've retrieved Maria's current queue. She is currently working on 3 active tasks, including 'Weekly Expense Report' (in progress) and 'Data Entry for Lead Gen' (pending). Would you like to view the details for any of these?


## Installation & Usage

To install and use the **Wing Assistant** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wing-assistant](https://vinkius.com/mcp/wing-assistant)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
