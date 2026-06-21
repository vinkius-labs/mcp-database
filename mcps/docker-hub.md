# Docker Hub MCP Server

Manage Docker images on Docker Hub — list repositories, browse tags, create repos and search for community images from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/docker-hub)

## Overview
**Category:** loved-by-devs
**Tools Count:** 10

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


## Available Tools
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


## Installation & Usage

To install and use the **Docker Hub** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/docker-hub](https://vinkius.com/mcp/docker-hub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
