# RubyGems MCP Server

Manage Ruby packages directly from your AI agent — search for gems, inspect versions, and track download statistics on RubyGems.org.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/rubygems)

## Overview
**Category:** developer-tools
**Tools Count:** 30

## Description
Connect to the **RubyGems** ecosystem to streamline your Ruby development workflow. This server allows your AI agent to interact with the world's largest Ruby package registry through natural conversation.

### What you can do

- **Gem Discovery** — Search for active gems and fetch detailed metadata for any specific Ruby package.
- **Version Management** — List all versions of a gem, identify the latest release, or track versions created within a specific timeframe.
- **Analytics & Stats** — Monitor total download counts and specific version statistics to understand gem popularity and usage.
- **Dependency Analysis** — Explore the ecosystem by listing reverse dependencies to see which gems rely on a specific package.
- **Owner & Security** — View gem owners and manage your own gems directly from your development environment.

### How it works

1. Subscribe to this server
2. Enter your RubyGems API Key
3. Start managing your Ruby dependencies from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Ruby Developers** — quickly check gem documentation, versions, and dependencies without leaving the terminal or IDE.
- **DevOps Engineers** — monitor package activity and download trends for critical infrastructure components.
- **Security Researchers** — analyze gem ownership and version history to audit supply chain risks.


## Available Tools
- **add_gem_owner**: Add an owner to a gem
- **create_webhook**: Use * for gem_name to apply to all gems.

Create a webhook
- **exchange_oidc_token**: Exchange an OIDC ID token for a short-lived API key
- **fire_webhook**: Test fire a webhook
- **get_api_key**: Retrieve your API key using HTTP Basic Auth
- **get_compact_index_info**: Returns a text-based format listing all versions of a specific gem
- **get_compact_index_names**: Returns a newline-delimited list of all gem names
- **get_compact_index_versions**: Returns a compact index of all gem names, versions, and info file MD5s
- **get_downloads**: Get total download count for all gems
- **get_gem_downloads**: Get download stats for a specific gem and version
- **get_gem_owners**: View all owners of a gem
- **get_gem**: Get basic information about a gem
- **get_gem_version_details_v2**: Returns detailed information for a specific gem version (API v2)
- **get_gem_versions**: Get all versions for a gem
- **get_just_updated_activity**: Pulls the 50 most recently updated gems
- **get_latest_activity**: Pulls the 50 most recently added gems
- **get_latest_gem_version**: Get the latest version of a gem
- **get_my_profile**: View your own profile info, including MFA status
- **get_owner_gems**: View all gems a user can push to
- **get_profile**: View basic user info
- **get_timeframe_versions**: Dates must be ISO8601 format.

Get versions created within a specific timeframe
- **list_my_gems**: Lists gems the user has push access to.

List all gems owned by the authenticated user
- **list_webhooks**: List registered webhooks
- **push_gem**: Pushes a new gem version using base64 encoded binary data.

Submit a built .gem file to RubyGems.org
- **remove_gem_owner**: Remove an owner from a gem
- **remove_webhook**: Remove a webhook
- **get_reverse_dependencies**: List gems that depend on the specified gem
- **search_gems**: org for gems matching the query. Results are paginated (30 per page).

Search for active gems
- **update_gem_owner**: Update an owner's role on a gem
- **yank_gem**: Yanks a specific version of a gem.

Remove a gem version from the index


## Installation & Usage

To install and use the **RubyGems** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rubygems](https://vinkius.com/mcp/rubygems)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
