# Unsplash MCP Server

Access millions of high-resolution images — search photos, manage collections, and track download statistics directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/unsplash-extended)

## Overview
**Category:** design-creative
**Tools Count:** 28

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


## Installation & Usage

To install and use the **Unsplash** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/unsplash-extended](https://vinkius.com/mcp/unsplash-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
