# Storyblok MCP Server

Connect your AI to Storyblok. Manage content spaces, craft data stories, and orchestrate headless CMS elements effortlessly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/storyblok)

## Overview
**Category:** developer-tools
**Tools Count:** 9

## Description
Integrate the powerful headless CMS capabilities of **Storyblok** directly into your conversational AI. Empower your content teams and developers to organically draft narratives, parse complex asset repositories, and orchestrate page component definitions without relying entirely on the visual editor. Bind your AI local context directly to your Storyblok environment securely, enabling programmatic schema generation and continuous iteration utilizing a streamlined conversational interface designed to accelerate creative velocity.

### What you can do

- **Space & Content Discovery** — Instantly list active enterprise environments utilizing `list_spaces` and fetch broad overarching overviews referencing stories via `list_stories`.
- **Content Construction** — Swiftly produce or update textual assets creating schemas directly from prompts invoking `create_content_story` and `update_content_story` systematically.
- **Asset & Structure Exploration** — Analyze media repositories via `list_assets` and precisely inspect available schema blueprints calling `list_components` to standardize development.
- **Risk Management** — Exercise safe administrative control over local projects, evaluating internal authorized operators implementing modifications using `list_space_users`.

### How it works

1. Establish the Storyblok MCP module as an integrated bridge on your chosen conversational interface.
2. In the MCP configurations, provide an authorized `STORYBLOK_TOKEN` to solidify local command execution effectively and encrypt connection pathways.
3. Prompt the agent: "Retrieve the exact block components deployed across our main Space, then formulate a new blog story formatted mathematically into JSON integrating standard textual boundaries."

### Who is this for?

- **Content Architects & SEO Managers** — Bulk-orchestrate and analyze complex content hierarchies swiftly deploying programmatic structural alterations iterating precisely on metadata parameters.
- **Frontend Developers** — Seamlessly query nested objects or retrieve component structural IDs programmatically isolating dependencies immediately via conversational context loops.
- **Agile Editors** — Systematically push localized iterations refining textual tone across multiple active platform drafts efficiently bypassing slow structural validations.


## Available Tools
- **create_content_story**: Provide a name, slug, and content JSON.

Creates a new story in a Storyblok space
- **delete_content_story**: This action is irreversible.

Permanently deletes a Storyblok story
- **get_story_details**: Retrieves details for a specific content story
- **list_assets**: Lists media assets in a Storyblok space
- **list_components**: Lists available content components
- **list_spaces**: Lists all accessible Storyblok spaces
- **list_stories**: Requires a space ID.

Lists content stories within a specific space
- **list_space_users**: Lists all users with access to a specific space
- **update_content_story**: Requires space and story IDs.

Updates fields of an existing Storyblok story


## Installation & Usage

To install and use the **Storyblok** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/storyblok](https://vinkius.com/mcp/storyblok)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
