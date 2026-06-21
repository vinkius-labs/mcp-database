# Clerk MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clerk-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/clerk-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/clerk-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Add production-ready authentication to your app with user management, SSO, multi-factor auth, and session handling out of the box.

## Description
Connect your **Clerk** account to any AI agent and take full control of your user authentication and multi-tenant management workflows through natural conversation.

### What you can do

- **User Orchestration** — List and manage all users registered in your application programmatically, including retrieving detailed high-fidelity profiles and contact info
- **Organization Architecture** — Access and monitor organizations and multi-tenant environments to coordinate team collaboration and access control in real-time
- **Invitation Lifecycle** — Programmatically send and track user invitations via email with custom redirect URLs to streamline your onboarding pipeline
- **Account Integrity** — Retrieve detailed user metadata and manage authentication status directly through your agent for instant operational reporting
- **Developer Visibility** — Access complete directories of auth-related resources to maintain a perfectly coordinated and secure development ecosystem

### How it works

1. Subscribe to this server
2. Retrieve your **Secret Key** from the Clerk Dashboard (API Keys section)
3. Start managing your user-centric applications from Claude, Cursor, or any MCP client

No more manual status checking or digging through user tables in the portal. Your AI acts as your dedicated auth architect and user management coordinator.

### Who is this for?

- **Developers & Admins** — instantly retrieve user profiles and manage multi-tenant setups using natural language commands
- **Operations Teams** — automate the dispatch of invitations and monitor organization growth without leaving your workspace
- **Customer Success** — check user authentication history and manage invitations through simple AI queries


## Available Tools
- **create_auth_invitation**: Send an invitation
- **create_auth_organization**: Create an organization
- **get_auth_user_details**: Get user details
- **list_auth_invitations**: List invitations
- **list_auth_organizations**: List organizations
- **list_auth_users**: List all users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clerk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all registered users in my Clerk application."

**🤖 AI Agent:**
> I've retrieved your user directory. You currently have 5 registered users, including 'John Doe' (ID: user_123) and 'Jane Smith'. Would you like the full profile metadata for any of them?

---

**👤 You:**
> "Send an invitation to 'newuser@example.com' with redirect to 'https://vinkius.com/start'."

**🤖 AI Agent:**
> Invitation dispatched! I've successfully sent an email invite to newuser@example.com. The invitation ID is 'inv_456'. I'll alert you as soon as they complete their registration.

---

**👤 You:**
> "Show all active organizations and their slugs."

**🤖 AI Agent:**
> Accessing multi-tenant data... You have 2 active organizations: 'Vinkius Enterprise' (Slug: vinkius-ent) and 'Beta Testers'. Would you like me to check for any pending invites within these teams?


## Installation & Usage

To install and use the **Clerk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clerk-alternative](https://vinkius.com/mcp/clerk-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
