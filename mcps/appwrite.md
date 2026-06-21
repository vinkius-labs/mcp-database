# Appwrite MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/appwrite)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Open-source backend-as-a-service — manage databases, storage, and users via AI.

## Description
Empower your AI agent to orchestrate your entire backend infrastructure with **Appwrite**. This unified server provides your agent with instant access to database management, user authentication auditing, and cloud storage monitoring. Your agent can instantly list your databases, audit document collections, and retrieve storage metrics without you ever touching the Appwrite console. Whether you are monitoring cloud function executions or managing project health, your agent acts as a dedicated backend developer through natural conversation.

### What you can do

- **Database Auditing** — List all databases and collections, and retrieve documents to analyze data structures.
- **User Management** — List and inspect project users to monitor registration trends and account statuses.
- **Storage Monitoring** — Access storage buckets and list files to audit assets and media distribution.
- **Function Insights** — Monitor cloud function configurations and retrieve recent execution logs for debugging.
- **System Health** — Get real-time health status for all integrated Appwrite services within your project.

### How it works

1. Subscribe to this server
2. Enter your Appwrite Project ID, API Key, and Endpoint
3. Start managing your backend infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Full-stack Developers** — instantly retrieve database schemas and audit users during the development cycle.
- **Backend Engineers** — automate infrastructure checks and monitor function executions through natural language.
- **Operations Managers** — track project health and storage usage without technical console logins.
- **SaaS Operators** — integrate Appwrite workflows into internal tools via an AI-guided interface.
- **Product Owners** — monitor user registration activity and database growth for organizational planning.


## Available Tools
- **get_health_status**: Check project health
- **list_storage_buckets**: List storage buckets
- **list_collections**: List collections in a database
- **list_databases**: List all databases
- **list_documents**: List documents in a collection
- **list_function_executions**: List function executions
- **list_bucket_files**: List files in a bucket
- **list_functions**: List cloud functions
- **list_users**: List project users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Appwrite** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all databases in my Appwrite project."

**🤖 AI Agent:**
> Retrieving your database directory... You currently have 3 active databases: 'production-db', 'staging-db', and 'analytics-store'. Which one would you like to inspect for collections?

---

**👤 You:**
> "Show the last 10 users registered in the project."

**🤖 AI Agent:**
> Fetching recent users... I've identified the 10 most recently registered accounts, including 'user_abc@email.com' and 'dev_test@domain.io'. I can provide their registration timestamps if needed.

---

**👤 You:**
> "Get execution logs for cloud function 'resize-image'."

**🤖 AI Agent:**
> Retrieving logs for 'resize-image'... The last 5 executions were successful, with an average duration of 150ms. I can display the specific status codes and output for each run.


## ❓ FAQ

**Q: How do I list all users in my Appwrite project?**
Use the `list_users` tool. It retrieves a comprehensive list of all registered users, allowing you to audit account statuses and registration activity.

**Q: Can I see the data within a specific collection?**
Yes! Use the `list_documents` tool by providing the Database ID and Collection ID. Your agent will fetch the documents stored in that collection for auditing and analysis.

**Q: How do I check if my Appwrite services are running correctly?**
Use the `get_health_status` tool. It provides a real-time overview of the health of various system components, ensuring your infrastructure is operational.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/appwrite](https://vinkius.com/mcp/appwrite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Appwrite** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `appwrite` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Appwrite** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "appwrite": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
