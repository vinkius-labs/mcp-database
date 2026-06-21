# Unsplash MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/unsplash-extended)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Access millions of high-resolution images — search photos, manage collections, and track download statistics directly from any AI agent.

## Description
Connect your **Unsplash** developer account to any AI agent and integrate the world's most popular open image library into your creative workflows.

### What you can do

- **Photo Discovery** — Search for specific imagery, list editorial feeds, or fetch random photos filtered by orientation, topics, or collections.
- **Collection Management** — Create, update, and organize photo collections. Add or remove images to curate your visual assets.
- **User Insights** — Retrieve public profiles, list user-specific uploads, and analyze engagement through detailed statistics.
- **Engagement** — Like or unlike photos and track downloads to comply with Unsplash API guidelines.
- **Topic Exploration** — Browse curated topics and fetch high-quality photos categorized by the Unsplash editorial team.

### How it works

1. Subscribe to this server
2. Enter your Unsplash Access Key (and optionally a Bearer Token for user-specific actions)
3. Start searching and managing images from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — find the perfect featured image for articles or social media posts without leaving the chat.
- **Designers** — quickly pull high-resolution inspiration or placeholders directly into your workspace.
- **Developers** — automate the retrieval of image metadata and statistics for application testing and content population.


## Available Tools
- **add_photo_to_collection**: Add a photo to a collection (requires user auth)
- **create_collection**: Create a new collection (requires user auth)
- **delete_collection**: Delete a collection (requires user auth)
- **get_collection_photos**: Get photos in a specific collection
- **get_collection**: Get a single collection by ID
- **get_me**: Get the authenticated user profile
- **get_photo_statistics**: Get statistics for a specific photo
- **get_photo**: Get a single photo by ID
- **get_random_photo**: Get one or more random photos
- **get_related_collections**: List related collections for a given collection ID
- **get_topic_photos**: Get photos for a specific topic
- **get_topic**: Get a single topic by ID or slug
- **get_user_statistics**: Get user download and view statistics
- **get_user**: Get a user public profile
- **like_photo**: Like a photo on behalf of the authenticated user
- **list_collections**: List all public collections
- **list_photos**: List photos from the editorial feed
- **list_topics**: List all topics
- **list_user_collections**: List collections created by a user
- **list_user_photos**: List photos uploaded by a user
- **remove_photo_from_collection**: Remove a photo from a collection (requires user auth)
- **search_collections**: Search collections by keyword
- **search_photos**: Search photos by keyword
- **search_users**: Search users by keyword
- **track_photo_download**: Track a photo download (Required for attribution)
- **unlike_photo**: Remove a like from a photo on behalf of the authenticated user
- **update_collection**: Update an existing collection (requires user auth)
- **update_me**: Update the authenticated user profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Unsplash** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 3 high-resolution photos of 'minimalist workspace' in landscape orientation."

**🤖 AI Agent:**
> I've found 3 minimalist workspace photos for you. [Photo 1: Clean desk with laptop], [Photo 2: Bright office with plants], [Photo 3: Zen wooden desk]. Would you like the download links for any of these?

---

**👤 You:**
> "Get a random photo from the 'Architecture' topic."

**🤖 AI Agent:**
> Here is a stunning random photo from the Architecture topic: [Image of a modern spiral staircase]. It was taken by 'UserXYZ'. Do you want to see more from this photographer?

---

**👤 You:**
> "Show me the statistics for the user 'unsplash_photographer'."

**🤖 AI Agent:**
> The user 'unsplash_photographer' has impressive engagement: 1.2M total views and 450k downloads across their 120 uploaded photos. Would you like to see their most popular collections?


## ❓ FAQ

**Q: Can I fetch a random photo based on a specific search term or topic?**
Yes! Use the `get_random_photo` tool. You can provide a `query` (like 'nature') or `topics` IDs to filter the random selection to exactly what you need.

**Q: Is it possible to create and manage my own photo collections via the AI?**
Absolutely. With a valid Bearer Token, you can use `create_collection`, `add_photo_to_collection`, and `remove_photo_from_collection` to curate your Unsplash assets directly through conversation.

**Q: How can I check the performance or popularity of a specific photo?**
You can use the `get_photo_statistics` tool by providing the photo ID. It will return detailed metrics including total views and downloads.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/unsplash-extended](https://vinkius.com/mcp/unsplash-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Unsplash** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `unsplash-extended` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Unsplash** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "unsplash-extended": {
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
