# RubyGems MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rubygems)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage Ruby packages directly from your AI agent — search for gems, inspect versions, and track download statistics on RubyGems.org.

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


## Available Tools (30)
- **create_webhook**: Use * for gem_name to apply to all gems.

Create a webhook
- **exchange_oidc_token**: Exchange an OIDC ID token for a short-lived API key
- **add_gem_owner**: Add an owner to a gem
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RubyGems** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for Ruby gems related to 'redis' and show me the top results."

**🤖 AI Agent:**
> I've searched RubyGems.org for 'redis'. The most relevant gems are 'redis' (the official client), 'redis-namespace', and 'redis-objects'. Would you like the full metadata for the main 'redis' gem?

---

**👤 You:**
> "What is the latest version of the 'rails' gem and when was it released?"

**🤖 AI Agent:**
> Using `get_latest_gem_version`, I found that the latest version of 'rails' is 7.1.3.2. It was released on February 21, 2024. Do you want to see the download statistics for this version?

---

**👤 You:**
> "Show me the download count for 'sidekiq' version 7.2.0."

**🤖 AI Agent:**
> I've retrieved the stats using `get_gem_downloads`. For 'sidekiq' version 7.2.0, there have been approximately 1.2 million downloads. The total downloads for all versions of Sidekiq exceed 150 million.


## ❓ FAQ

**Q: Can I see which gems depend on a specific gem?**
Yes! Use the `get_reverse_dependencies` tool with the gem name. It will return a list of all gems on RubyGems.org that list that gem as a dependency.

**Q: How do I check my own gems and their status?**
By providing your API key, you can use the `list_my_gems` tool. This will display all gems where you have push access and ownership rights.

**Q: Can I get the full version history of a package?**
Absolutely. The `get_gem_versions` tool retrieves every published version of a specific gem, allowing you to audit changes and release frequency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rubygems](https://vinkius.com/mcp/rubygems)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **RubyGems** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rubygems` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **RubyGems** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rubygems": {
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
