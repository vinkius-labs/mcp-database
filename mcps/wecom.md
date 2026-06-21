# WeCom / 企业微信 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wecom)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Enterprise communication and management platform — manage departments, users, and messages via AI.

## Description
Empower your AI agent to orchestrate your enterprise operations with **WeCom** (Enterprise WeChat), the dominant business communication platform in China. By connecting WeCom to your agent, you transform complex organization management and internal communication into a natural conversation. Your agent can instantly list departments, retrieve employee profiles, monitor attendance data, and even send messages to staff members without you needing to navigate the comprehensive WeCom Admin Backend. Whether you are managing a large-scale workforce or a specific internal application, your agent acts as a real-time operations assistant, keeping your data accurate and your team aligned.

### What you can do

- **Organization Orchestration** — List all departments and retrieve detailed employee profiles across your company.
- **Staff Communication** — Send instant text messages to any user in your organization directly through the chat interface.
- **Attendance Monitoring** — Retrieve real-time check-in data for employees to audit workforce activity.
- **Tag & Group Management** — Browse organization tags and identify users belonging to specific functional groups.
- **Application Insights** — Retrieve metadata about your internal apps, including custom menu configurations.

### How it works

1. Subscribe to this server
2. Enter your WeCom Corp ID, App Secret, and Agent ID
3. Start managing your enterprise operations through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **HR Managers** — monitor team attendance and manage employee records through natural language queries.
- **Internal Operations** — coordinate staff communication and audit organizational structures via a unified AI interface.
- **IT Administrators** — monitor application agents and retrieve system metadata without manual technical overhead.
- **WeCom Users** — integrate your existing enterprise workflows into your AI-driven daily routines.


## Available Tools
- **get_app_details**: Get application agent details
- **get_attendance_data**: Get employee attendance/checkin data
- **get_department**: Get department info
- **get_tag_users**: Get users with a specific tag
- **get_user**: Get user details
- **list_departments**: List all departments
- **list_menu**: Get app custom menu
- **list_tags**: List all organization tags
- **list_users**: List users in a department
- **send_message**: Send a text message to a user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WeCom / 企业微信** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all departments in our organization."

**🤖 AI Agent:**
> I've retrieved the organizational structure for WeCom. You have 5 primary departments, including 'Engineering', 'Marketing', and 'Sales'. Which one would you like to see the users for?

---

**👤 You:**
> "Send a message to user 'Mario' saying 'The deployment is complete'."

**🤖 AI Agent:**
> Done! I've sent your message to Mario through the WeCom application. He has been notified that the deployment is complete.

---

**👤 You:**
> "Show me the attendance data for 'mario,renato' from today."

**🤖 AI Agent:**
> I've retrieved the check-in data for the specified users. Mario punched in at 9:00 AM, and Renato punched in at 8:45 AM. Both are currently marked as active in the system.


## ❓ FAQ

**Q: How do I find my WeCom Corp ID and Secret?**
Log in to the WeCom Admin Backend. Your Corp ID is in [My Company] → [Company Profile]. Your App Secret and Agent ID are in [Apps] → select your application.

**Q: Can I read attendance records for a group of users?**
Yes. Use the `get_attendance_data` tool. You will need to provide a start time, end time, and a comma-separated list of user IDs to retrieve the records.

**Q: Does my application need specific permissions for messages?**
Yes. Ensure your application has 'Messaging' permissions enabled in the WeCom Admin Backend and that the 'Trusted IPs' for your server are correctly configured.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wecom](https://vinkius.com/mcp/wecom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WeCom / 企业微信** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `wecom` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WeCom / 企业微信** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wecom": {
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
