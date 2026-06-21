# Storyblok MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/storyblok)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Connect your AI to Storyblok. Manage content spaces, craft data stories, and orchestrate headless CMS elements effortlessly.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Storyblok** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the recent articles from my Storyblok space and detail their structural components."

**🤖 AI Agent:**
> Connected to your Storyblok space.
**Recent Stories (`list_stories`)**:
- `Introduction to LLMs`
- `Marketing Automation Update`
- `Platform Change-log`

Inspecting component structure via `get_story_details`:
- Components: `hero_banner`, `rich_text`, `call_to_action`. Ready for modifications.

---

**👤 You:**
> "List the structure blueprints by calling list_components and then formulate a new JSON to create a blog story."

**🤖 AI Agent:**
> Analyzing current schemas...

**Available Components (`list_components`)**:
- `article_body`
- `media_header`

Structuring the payload...
**Created Story (`create_content_story`)**:
Successfully published the new blog story 'Future Tech' into the content repository.

---

**👤 You:**
> "List all multimedia assets in my Storyblok space and display their URLs."

**🤖 AI Agent:**
> Scanning the media repository...

**Assets Discovered (`list_assets`)**:
- `product_demo.mp4` -> `//a.storyblok.com/.../demo.mp4`
- `hero_bg.jpg` -> `//a.storyblok.com/.../hero.jpg`

These assets are ready to be integrated into your active story components.


## ❓ FAQ

**Q: How does the AI validate JSON payloads before creating content?**
Instruct the agent to call `list_components` first. It returns the exact field names and types each component expects, so the AI builds a compliant JSON payload before calling `create_content_story`.

**Q: Can the agent accidentally delete entire spaces?**
No. `delete_content_story` targets a single story by ID — it cannot perform recursive or bulk deletions. For extra safety, use a token scoped with limited write permissions.

**Q: What content types can I manage through this integration?**
Stories (pages, articles, blog posts), media assets (images, videos, documents), component definitions, and space-level settings. Use `list_stories`, `list_assets`, and `list_components` to explore your content.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/storyblok](https://vinkius.com/mcp/storyblok)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Storyblok** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `storyblok` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Storyblok** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "storyblok": {
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
