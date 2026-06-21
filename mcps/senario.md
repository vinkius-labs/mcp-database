# Senar.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/senario)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Detect and respond to security threats with AI-powered SIEM that correlates events across your infrastructure in real time.

## Description
Connect your **Senar.io** account to any AI agent and take full control of your augmented reality training orchestration through natural conversation. Senar.io provides a premier platform for VR/AR simulators, and this integration allows you to retrieve training metadata, assign simulators to users, and monitor performance results directly from your chat interface.

### What you can do

- **User & Trainee Orchestration** — List all managed users and retrieve detailed profile metadata, including creating and assigning users to collections programmatically.
- **Simulator Lifecycle Management** — Access and monitor your AR simulator collections and retrieve detailed module metadata directly from the AI interface.
- **Activity & Performance Intelligence** — Retrieve real-time training activity logs, including attempts, success rates, and duration data via natural language.
- **Session & History Control** — Access historical user session history to ensure your training compliance and skill development are always synchronized.
- **Operational Monitoring** — Track organization-wide training health and manage collection assignments using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your Senar Studio Username and Password
3. Start managing your AR training workflows from Claude, Cursor, or any MCP-compatible client

No more manual user imports or spreadsheet result tracking. Your AI acts as a dedicated training coordinator or LMS assistant.

### Who is this for?

- **Training Managers** — quickly retrieve trainee results and monitor simulator usage without switching apps.
- **L&D Teams** — automate the assignment of training modules and track skill acquisition via natural conversation.
- **Safety Officers** — streamline the retrieval of session records and monitor certification compliance directly within the chat.


## Available Tools (9)
- **add_content**: Add content to a collection
- **create_user_and_assign**: Create a new user and assign them to an AR collection
- **get_activity_data**: Get detailed training activity results
- **get_collection_details**: Get details for a content collection
- **get_progress**: Get learning progress for a user
- **get_user_sessions**: List all sessions for a specific user
- **get_user_details**: Get details for a specific user
- **list_collections**: List all AR simulator collections
- **list_users**: List all users in your organization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Senar.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active collections in my Senar account."

**🤖 AI Agent:**
> I've retrieved your collections. You have 3 active simulator groups: 'Forklift Safety', 'Hazard Identification', and 'First Aid'. Which one would you like to assign users to?

---

**👤 You:**
> "Show me the learning progress for all users in the Engineering team with completion rates."

**🤖 AI Agent:**
> Engineering team: 24 users. Average completion: 67%. Top performers: Sarah Chen (92%, 12 courses completed), James Park (88%, 10 courses). "Cloud Architecture" collection: 83% team completion. "Security Best Practices": 71% completion (mandatory, deadline next week). "Advanced Kubernetes": 45% (newly assigned). "Leadership Fundamentals": 34% (optional). 5 users have not logged in this month. 3 certifications earned this week. Total learning hours: 456 hours. Average session duration: 23 minutes.

---

**👤 You:**
> "Add a new training module to the Security collection and assign it to all engineering team members."

**🤖 AI Agent:**
> Training module added: "Incident Response Procedures 2025". Collection: Security Best Practices. Content: 8 lessons, 2 quizzes, 1 simulation exercise. Estimated duration: 2.5 hours. Assigned to: 24 engineering team members. Deadline: June 15, 2025. Notification emails sent to all assignees. Prerequisite set: "Security Fundamentals" (auto-verified, 22 of 24 have completed). 2 users need to complete prerequisites first. Progress tracking enabled. Completion certificate: auto-generated upon passing quiz.


## ❓ FAQ

**Q: Can my AI automatically assign a new user to a specific simulator collection?**
Yes! Use the `create_user_and_assign` tool. Provide the user details and the Collection ID, and your agent will create the record and grant access instantly.

**Q: How do I find a collectionId for my simulators?**
In Senar Studio, open your collection; the ID is the numeric value at the end of the URL (e.g., .../Collections/Edit/123).

**Q: Are training results available in real-time?**
Yes, as soon as a trainee completes a session in the AR simulator, the data is pushed to the API and accessible via the `get_activity_data` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/senario](https://vinkius.com/mcp/senario)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Senar.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `senario` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Senar.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "senario": {
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
