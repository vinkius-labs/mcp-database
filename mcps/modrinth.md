# Modrinth MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/modrinth)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/modrinth-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/modrinth-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Search and manage Minecraft projects via Modrinth — discover mods, resource packs, and plugins directly from your AI agent.

## Description
Connect to the **Modrinth** ecosystem through your AI agent to discover and manage Minecraft mods, resource packs, and plugins using natural conversation.

### What you can do

- **Project Discovery** — Search for projects using advanced filters for game versions, loaders, and categories.
- **Version Management** — List all available versions for any project and get detailed download links and metadata.
- **Dependency Tracking** — Automatically identify other projects that a mod depends on to function correctly.
- **User & Team Insights** — View public profiles, search for creators, and list team members for any project.
- **Community Metrics** — Monitor project popularity by listing followers and viewing detailed metadata including download counts.
- **Direct Download Info** — Access specific version files, hashes, and loader compatibility details.

### How it works

1. Subscribe to this server
2. (Optional) Enter your Modrinth Personal Access Token for higher rate limits
3. Start exploring Minecraft projects with Claude, Cursor, or any MCP client

### Who is this for?

- **Minecraft Players** — find the latest optimization or content mods without leaving your chat.
- **Server Admins** — quickly check for updates, dependencies, and team info for your server plugins.
- **Developers** — inspect project metadata, user profiles, and version histories while working on integrations.


## Available Tools
- **get_project_dependencies**: Get project dependencies
- **get_project**: Get detailed Modrinth project info
- **get_team_members**: List project team members
- **get_user_profile**: Get user profile info
- **get_version**: Get specific version details
- **list_project_followers**: List project followers
- **list_user_projects**: List projects by a user
- **list_versions**: List versions of a Modrinth project
- **search_projects**: You can include game versions (e.g., 1.20.1) or loaders (e.g., Fabric) in your query.

Search for Minecraft projects on Modrinth
- **search_users**: Search for Modrinth users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Modrinth** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for optimization mods for Minecraft 1.20.1 using Fabric."

**🤖 AI Agent:**
> I've searched Modrinth and found several optimization mods for Fabric 1.20.1. The top results include 'Sodium' (a modern rendering engine), 'Lithium' (game logic optimization), and 'Indium' (Sodium compatibility layer). Would you like to see the versions available for Sodium?

---

**👤 You:**
> "Who are the developers of the Sodium mod?"

**🤖 AI Agent:**
> The Sodium development team includes several key contributors. The primary authors associated with the project are 'jellysquid3' and members of the CaffeineMC organization. Would you like to see other projects by jellysquid3?

---

**👤 You:**
> "What does the 'Iris Shaders' mod depend on?"

**🤖 AI Agent:**
> I've checked the dependencies for Iris Shaders. It primarily requires 'Sodium' to function. It also has optional dependencies like 'Indium' for better compatibility with other mods. Shall I retrieve the latest version details for Sodium as well?


## Installation & Usage

To install and use the **Modrinth** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/modrinth](https://vinkius.com/mcp/modrinth)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
