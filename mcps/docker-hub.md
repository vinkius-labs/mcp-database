# Docker Hub MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/docker-hub)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage Docker images on Docker Hub — list repositories, browse tags, create repos and search for community images from any AI agent.

## Description
Connect your **Docker Hub** account to any AI agent and manage your container images through natural conversation.

### What you can do

- **Repository Management** — List, create, update and delete Docker image repositories
- **Tag Discovery** — Browse available image tags with versions, sizes and architecture info
- **Account Info** — View your user profile, organizations and repository statistics
- **Image Search** — Search for public Docker images by name or description
- **Pull Stats** — Monitor pull counts and repository popularity metrics

### How it works

1. Subscribe to this server
2. Enter your Docker Hub Access Token
3. Start managing your container images from Claude, Cursor, or any MCP-compatible client

No more navigating the Docker Hub website to check tags or manage repositories. Your AI acts as a dedicated container registry assistant.

### Who is this for?

- **DevOps Engineers** — quickly check available image tags, monitor pull stats and manage repository settings
- **Developers** — search for community images, discover correct tag versions and verify image metadata
- **Platform Teams** — audit repository access, track organization membership and manage image visibility


## Available Tools (10)
- **create_repository**: Requires the namespace (your username or org) and repository name. Optionally set a description and visibility (public/private). Returns the created repository.

Create a new Docker Hub repository
- **delete_repository**: Provide the namespace and repository name. WARNING: this action is irreversible.

Delete a Docker Hub repository
- **get_repository**: Provide the namespace (username/org) and repository name.

Get details for a specific Docker Hub repository
- **get_tag**: Provide the namespace, repository name and tag name (e.g. "latest", "v1.2.3").

Get details for a specific image tag
- **get_user**: Returns username, email, full name, location, company and account type. Use this to verify your access token is working correctly.

Get the authenticated Docker Hub user info
- **list_organizations**: Each organization includes its name, full name, type and creation date.

List organizations the user belongs to
- **list_repositories**: Each repository shows its name, namespace, description, star count, pull count, visibility (public/private) and last updated date. Optionally set pagination parameters.

List Docker Hub repositories (images)
- **list_tags**: Each tag shows the tag name, image size, last pushed date and digest. Useful for discovering available image versions.

List tags for a Docker Hub repository
- **search_repositories**: Returns matching repos with their namespace, name, star count, pull count and description. Useful for discovering community images.

Search for Docker Hub repositories
- **update_repository**: Provide the namespace, repository name and a JSON object with fields to update (e.g. {"description": "New description", "is_private": true}). Only provided fields will be modified.

Update a Docker Hub repository


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Docker Hub** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Docker repositories."

**🤖 AI Agent:**
> I found 5 repositories: 'myapp-api' (12K pulls, public), 'myapp-web' (8K pulls, public), 'myapp-worker' (private), 'base-image' (25K pulls, public) and 'test-env' (private). Would you like details on any of them?

---

**👤 You:**
> "Show me all available tags for the nginx official image."

**🤖 AI Agent:**
> The nginx repository has 200+ tags. Latest versions include: 'latest' (187MB, pushed 2 days ago), '1.25-alpine' (42MB), '1.25.3' (187MB), '1.25.3-alpine' (42MB), and '1.24-perl' (205MB). Would you like details on a specific tag?

---

**👤 You:**
> "Search for official Python images on Docker Hub."

**🤖 AI Agent:**
> Found the official 'python' image with 1.2B+ pulls. Also found related images: 'python:alpine' (lightweight, 50MB), 'python:slim' (minimal, 130MB), and community images like 'python:3.12-slim'.


## ❓ FAQ

**Q: How do I get a Docker Hub access token?**
Log in to [**hub.docker.com**](https://hub.docker.com/settings/security), go to **Settings > Security**, click **New Access Token**, give it a name and copy the token immediately — it starts with `dckr_pat_` and won't be shown again.

**Q: Can I create private repositories?**
Yes! Use `create_repository` with `is_private` set to "true". Note that free Docker Hub accounts have a limited number of private repositories. Check your account plan for private repo limits.

**Q: Can I search for public Docker images?**
Yes! Use `search_repositories` with a query like "nginx", "python" or "node". Results include the namespace, name, star count, pull count and description for each matching image. This is useful for discovering community images before pulling them.

**Q: Can I see all tags for an image?**
Yes! Use `list_tags` with the namespace and repository name. Returns all available tags with their image sizes, last pushed dates and digests. Useful for finding the correct version to pull.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/docker-hub](https://vinkius.com/mcp/docker-hub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Docker Hub** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `docker-hub` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Docker Hub** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "docker-hub": {
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
