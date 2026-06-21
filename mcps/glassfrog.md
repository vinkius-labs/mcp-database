# GlassFrog MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/glassfrog)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Manage Holacracy circles, roles, and tactical projects via AI agents with GlassFrog.

## Description
Connect your **GlassFrog** organization to any AI agent to automate your Holacracy governance and tactical operations through the Model Context Protocol (MCP). GlassFrog is the premier platform for self-management and organizational clarity. This MCP server enables you to retrieve circle structures, role definitions, project lists, and performance metrics directly through natural conversation.

### Key Features

- **Organizational Oversight** — List all circles and role definitions, retrieving detailed purposes and accountabilities for every role in the organization.
- **Tactical Project Management** — Access and list tactical projects, and programmatically create new projects within specific circles from your chat interface.
- **Governance Transparency** — Retrieve circle policies and governance records to understand the rules and constraints of your organization.
- **Performance Metrics** — Access defined metrics and checklist items to track organizational health and tactical progress.
- **Workforce Collaboration** — List all organization members and search for specific people by email to verify role assignments.
- **Real-time Synchronization** — Keep your Holacracy data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your GlassFrog API Key (found in User Profile > Settings > API Keys)
3. Start managing your Holacracy organization from Claude, Cursor, or any MCP client

### Who is this for?

- **Lead Links & Facilitators** — quickly check circle accountabilities or list tactical projects without manual dashboard navigation.
- **Operations Managers** — get a real-time overview of organizational metrics and policies via simple AI commands.
- **Self-Managed Teams** — automate the tracking of next actions and project statuses for better tactical alignment.


## Available Tools
- **verify_api_connection**: Check connection
- **create_new_project**: Add a project
- **find_member_by_email**: Search member
- **get_circle_summary**: Get circle overview
- **list_role_assignments**: List assignments
- **list_checklist_items**: List checklists
- **list_holacracy_circles**: List all circles
- **list_circle_metrics**: List metrics
- **list_org_members**: List people
- **list_circle_policies**: List policies
- **list_tactical_projects**: List all projects
- **list_holacracy_roles**: List role definitions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GlassFrog** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active circles in my organization."

**🤖 AI Agent:**
> Retrieving circles... I found 5 active circles, including 'General Circle' (ID: 1), 'Engineering', and 'Marketing'. Would you like the roles for any of them?

---

**👤 You:**
> "What are the accountabilities for the 'Product Manager' role?"

**🤖 AI Agent:**
> Fetching role details... The Product Manager role (Circle: Engineering) has 3 accountabilities: 1. Defining product strategy, 2. Prioritizing the roadmap, 3. Gathering user feedback.

---

**👤 You:**
> "Show me the current tactical metrics for the 'Marketing' circle (ID: 123)."

**🤖 AI Agent:**
> Retrieving metrics... For the Marketing circle, I found 2 active metrics: 'Monthly Active Users' and 'Ad Spend Efficiency'. Both were last updated 2 days ago.


## ❓ FAQ

**Q: How do I get an API Key for GlassFrog?**
Log in to your GlassFrog account, click on your profile avatar, go to 'Settings', and then 'API Keys' to generate or copy your token.

**Q: What is a Circle in GlassFrog?**
A Circle is an organizational unit in Holacracy that groups together related roles and responsibilities to achieve a specific purpose.

**Q: Can I create new projects via the agent?**
Yes! Use the 'create_new_project' tool. You will need to provide a description and the ID of the Circle where the project should be added.

**Q: How do I find a Circle ID?**
Use the 'list_holacracy_circles' tool. The agent will return all available circles along with their unique IDs and names.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/glassfrog](https://vinkius.com/mcp/glassfrog)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GlassFrog** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `glassfrog` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GlassFrog** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "glassfrog": {
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
