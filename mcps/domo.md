# Domo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/domo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Manage Domo users and groups directly from your AI agent — create, update, and delete users, or organize them into groups for better governance.

## Description
Connect your **Domo** instance to any AI agent to streamline user administration and group management through natural language.

### What you can do

- **User Administration** — Create new users with specific roles (Admin, Privileged, Participant), update existing profiles, or remove users from the system.
- **Group Management** — Create organizational groups to manage access at scale.
- **Membership Control** — Seamlessly add or remove users from specific Domo groups to maintain security and collaboration standards.

### How it works

1. Subscribe to this server
2. Enter your Domo Access Token
3. Start managing your BI environment from Claude, Cursor, or any MCP client

### Who is this for?

- **BI Administrators** — Quickly provision or deprovision users without navigating complex admin panels.
- **Team Leads** — Organize team members into groups for shared dashboard access.
- **IT Operations** — Automate user lifecycle management within the Domo ecosystem.


## Available Tools (6)
- **create_user**: Optionally sends an invite email.

Create a new Domo user
- **remove_user_from_group**: Remove a user from a Domo group
- **add_user_to_group**: Add a user to a Domo group
- **create_group**: Create a new Domo group
- **delete_user**: Delete a Domo user
- **update_user**: Update an existing Domo user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Domo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new Domo user for Alice Smith (alice@company.com) as a 'Privileged' user."

**🤖 AI Agent:**
> I've initiated the creation of Alice Smith's account with the 'Privileged' role. An invitation email has been sent to alice@company.com.

---

**👤 You:**
> "Update user ID 55021 to have the job title 'Senior Analyst' and location 'New York'."

**🤖 AI Agent:**
> User 55021 has been updated. Their profile now reflects the title 'Senior Analyst' in the New York office.

---

**👤 You:**
> "Add user 10293 to the 'Data Science' group (ID 9982)."

**🤖 AI Agent:**
> User 10293 has been successfully added to the 'Data Science' group. They now have access to the group's shared resources.


## ❓ FAQ

**Q: Can I automatically send an invitation email when creating a new user?**
Yes. When using the `create_user` tool, the `sendInvite` parameter defaults to true, which triggers an invitation email to the new user's address.

**Q: How do I change a user's role to Admin?**
Use the `update_user` tool and provide the user's unique ID along with the `role` parameter set to 'Admin'.

**Q: Is it possible to remove a user from a specific group without deleting their account?**
Absolutely. Use the `remove_user_from_group` tool with the corresponding `group_id` and `user_id`. This only modifies group membership.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/domo](https://vinkius.com/mcp/domo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Domo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `domo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Domo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "domo": {
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
