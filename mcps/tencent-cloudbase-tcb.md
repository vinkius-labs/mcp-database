# Tencent CloudBase / 腾讯云开发 TCB MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tencent-cloudbase-tcb)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tencent-cloudbase-tcb-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tencent-cloudbase-tcb-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

China's dominant serverless platform — orchestrate cloud functions, databases, and storage via AI.

## Description
Empower your AI agent to orchestrate your serverless infrastructure and backend resources with **Tencent CloudBase** (云开发), the premier BaaS platform in China. By connecting TCB to your agent, you transform complex cloud function management, database auditing, and storage orchestration into a natural conversation. Your agent can instantly retrieve function lists, invoke cloud logic with custom data, query NoSQL collections, and monitor environment quotas without you ever needing to navigate the comprehensive Tencent Cloud Console. Whether you are managing miniapp backends or coordinating high-volume digital automation, your agent acts as a real-time serverless operations assistant, providing accurate results from a single, authorized source.

### What you can do

- **Function Orchestration** — List cloud functions, retrieve detailed metadata, and invoke logic directly through the agent.
- **Database Auditing** — List database collections and execute complex queries on your cloud NoSQL data.
- **Storage Management** — List and audit storage buckets and monitor file resources within your environment.
- **User Management** — Retrieve lists of authenticated users registered in your TCB environment.
- **Operational Monitoring** — Verify project connectivity, active regions, and monitor free quota usage to ensure stability.

### How it works

1. Subscribe to this server
2. Enter your Tencent Cloud SecretId, SecretKey, Region, and EnvId
3. Start managing your serverless backend through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Miniapp & Web Developers** — automate routine backend audits and trigger cloud logic through natural language.
- **DevOps Engineers** — monitor environment health and audit resource usage directly from your workspace.
- **Developers** — integrate professional-grade serverless capabilities into your AI-driven daily routines.
- **Tencent Cloud Power Users** — integrate your existing TCB projects into your AI-driven daily routines.


## Available Tools
- **get_environment_info**: Get TCB environment details
- **get_function_metadata**: Get function details
- **invoke_cloud_function**: Trigger cloud function
- **list_auth_users**: List authenticated users
- **list_cloud_functions**: List cloud functions
- **list_collections**: List database collections
- **list_tcb_buckets**: List storage buckets
- **query_cloud_db**: Query cloud database


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tencent CloudBase / 腾讯云开发 TCB** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all cloud functions in our 'prod-8821' environment."

**🤖 AI Agent:**
> I've retrieved the cloud function list for environment `prod-8821`. You have 12 active functions, including 'OrderProcessor' (Node.js 16) and 'UserSync' (Python 3.7). Would you like me to trigger one of these functions for you?

---

**👤 You:**
> "Query the 'Users' collection for all documents where 'status' is 'active'."

**🤖 AI Agent:**
> I've executed the database query on the 'Users' collection. I found 45 active users. Should I retrieve the full details for the first few users or check your remaining storage quota?

---

**👤 You:**
> "Show me the configuration and quota usage for our TCB environment."

**🤖 AI Agent:**
> I've retrieved your environment summary. Your TCB instance is running in 'ap-shanghai' and is currently 'NORMAL'. You have used 45% of your free storage quota and 12% of your monthly function invocations. Would you like me to audit your VPC settings?


## Installation & Usage

To install and use the **Tencent CloudBase / 腾讯云开发 TCB** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tencent-cloudbase-tcb](https://vinkius.com/mcp/tencent-cloudbase-tcb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
