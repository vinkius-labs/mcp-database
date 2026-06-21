# Domo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/domo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/domo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/domo-mcp)
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


## Available Tools
- **add_user_to_group**: Add a user to a Domo group
- **create_group**: Create a new Domo group
- **create_user**: Optionally sends an invite email.

Create a new Domo user
- **delete_user**: Delete a Domo user
- **remove_user_from_group**: Remove a user from a Domo group
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


## Installation & Usage

To install and use the **Domo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/domo](https://vinkius.com/mcp/domo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
