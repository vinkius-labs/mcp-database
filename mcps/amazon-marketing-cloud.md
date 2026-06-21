# Amazon Marketing Cloud MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amazon-marketing-cloud)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/amazon-marketing-cloud-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/amazon-marketing-cloud-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Advanced advertising analytics — execute SQL queries and monitor workflows via AI.

## Description
Connect your **Amazon Marketing Cloud (AMC)** instance to your AI agent to unlock professional cross-channel advertising analytics. From defining SQL-based workflows to executing ad-hoc queries and retrieving secure download URLs for your reports, your agent handles your AMC data pipelines through natural conversation.

### What you can do

- **Workflow Orchestration** — List, retrieve, and manage saved SQL workflows to standardize your analytics
- **Execution Management** — Trigger new workflow executions or ad-hoc SQL queries and monitor their processing status
- **Results Retrieval** — Securely fetch S3 download URLs for completed execution outputs directly from chat
- **Task Oversight** — Audit recent execution history and cancel long-running or stalled queries
- **Data Insights** — Quickly organize and trigger complex multi-touch attribution queries without navigating the AWS console

### How it works

1. Subscribe to this server
2. Enter your AMC Instance ID, Amazon Ads Client ID, Client Secret, Refresh Token, Region, and Profile ID
3. Start managing your SQL workflows and generating analytics through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — automate the execution of recurring SQL queries and retrieve results effortlessly
- **Media Buyers** — run ad-hoc queries to understand multi-channel attribution and audience overlap
- **Marketing Engineers** — manage AMC workflow configurations and verify API execution statuses on the fly
- **Advertising Strategists** — request complex analytics reports via simple chat commands for external visualization


## Available Tools
- **list_workflows**: List AMC workflows
- **create_workflow**: Create an AMC workflow
- **get_workflow_details**: Get workflow details
- **update_workflow**: Update an AMC workflow
- **delete_workflow**: Delete an AMC workflow
- **list_executions**: List workflow executions
- **create_execution**: Execute an AMC query
- **get_execution_status**: g. PENDING, COMPLETED).

Check execution status
- **delete_execution**: Cancel an execution
- **get_execution_download_urls**: Get execution download URLs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amazon Marketing Cloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my saved AMC workflows."

**🤖 AI Agent:**
> I've retrieved your saved workflows. You have 5 workflows available, including 'Campaign Overlap Analysis' and 'Path to Conversion'. Which workflow would you like to execute?

---

**👤 You:**
> "Check the status of execution ID 'exec-12345'."

**🤖 AI Agent:**
> I've checked the status for execution exec-12345. The status is 'COMPLETED'. The query finished successfully. Would you like me to retrieve the download URL for the results?

---

**👤 You:**
> "Execute workflow 'wkfl-98765' for the last 7 days."

**🤖 AI Agent:**
> I have successfully triggered the execution for workflow wkfl-98765 for the requested time window. The Execution ID is 'exec-abc-123'. Because AMC processes queries asynchronously, it is currently PENDING. I will check the status for you shortly.


## Installation & Usage

To install and use the **Amazon Marketing Cloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amazon-marketing-cloud](https://vinkius.com/mcp/amazon-marketing-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
