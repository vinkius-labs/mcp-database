# Immich (Google Photos Alternative) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/immich-google-photos-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [image-video](../categories/image-video.md)

Manage your self-hosted Immich photo and video library — list assets, organize albums, and handle user administration via AI.

## Description
Connect your self-hosted **Immich** instance to any AI agent and take full control of your digital media library through natural conversation. Immich is the leading open-source alternative to Google Photos, and this MCP server allows you to interact with your assets, albums, and server settings seamlessly.

### What you can do

- **Asset Management** — List, fetch, update, and delete photos or videos. You can even upload new media directly from your local environment.
- **Album Organization** — Create and manage albums to keep your memories organized without manual clicking.
- **User & Person Administration** — List and manage users, persons (faces), and tags to maintain a clean and searchable library.
- **Server Monitoring** — Instantly check your Immich server version and status to ensure everything is running smoothly.

### How it works

1. Subscribe to this server
2. Enter your Immich Instance URL and API Key
3. Start managing your media library from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Self-Hosters** — Manage your private cloud media library without leaving your workspace.
- **Content Creators** — Quickly find, update, or upload assets for projects using natural language.
- **System Administrators** — Monitor server health and manage user accounts across your Immich instance efficiently.


## Available Tools (26)
- **get_person**: Provide the person’s UUID as the required input.

Get details for a specific person
- **get_user**: Pass the user UUID to identify the target user.

Get details for a specific user
- **list_assets**: List all assets (photos/videos) in Immich
- **list_persons**: Use this to find a person’s unique identifier.

List all recognized persons in Immich
- **list_tags**: Use this to find a tag’s unique identifier.

List all tags in Immich
- **get_server_info**: Get Immich server version and status information
- **update_asset**: g., isFavorite).

Update an existing Immich asset
- **update_person**: Supply the person’s UUID and the data payload.

Update an existing person (e.g., change name)
- **update_tag**: Supply the tag’s UUID and the data payload.

Update an existing tag
- **upload_asset**: Upload a new photo or video to Immich
- **get_tag**: Pass the tag’s UUID to fetch the information.

Get details for a specific tag
- **create_album**: Supply a JSON payload containing the album details.

Create a new album
- **list_albums**: Do not specify any parameters.

List all albums in Immich
- **create_user**: Supply a JSON payload with the required user details.

Create a new user
- **delete_album**: Use the album UUID to identify the target album.

Delete an album
- **delete_person**: Use the person’s UUID to identify the record.

Delete a person record
- **delete_tag**: Provide the UUID of the tag to be deleted.

Delete a tag
- **delete_user**: Provide the UUID of the user to be deleted.

Delete a user
- **get_album**: Provide the album UUID as the required ID.

Get details for a specific album
- **get_asset**: Get details for a specific Immich asset
- **create_tag**: Supply a JSON payload containing the tag details.

Create a new tag
- **list_users**: No authentication is required for this query.

List all users in Immich
- **create_person**: Supply a JSON payload with the person’s details.

Create a new person record
- **delete_asset**: Delete an Immich asset
- **update_album**: Supply both the album ID and the data payload.

Update an existing album
- **update_user**: Provide the user ID and the data payload.

Update an existing user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Immich (Google Photos Alternative)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my photos in Immich."

**🤖 AI Agent:**
> I've retrieved your assets. You have 150 photos and videos available. Would you like to see the details of the most recent one?

---

**👤 You:**
> "Create a new album called 'Summer Vacation 2024'."

**🤖 AI Agent:**
> The album 'Summer Vacation 2024' has been successfully created with UUID: 8f2d... You can now start adding assets to it.

---

**👤 You:**
> "Get the details for asset 550e8400-e29b-41d4-a716-446655440000."

**🤖 AI Agent:**
> Inspecting asset... This is a JPEG image taken on 2023-08-15. It is currently marked as a favorite and is part of the 'Travel' album.


## ❓ FAQ

**Q: How can I check if my Immich server is online and see its version?**
You can use the `get_server_info` tool. It will return the current version of the Immich server and its operational status.

**Q: Is it possible to upload a photo directly from my computer using this server?**
Yes! Use the `upload_asset` tool by providing the absolute local file path. The AI will handle the multipart upload to your Immich instance.

**Q: Can I create a new album to organize my photos?**
Absolutely. Use the `create_album` tool and provide a JSON payload with the `albumName`. You can also manage existing ones with `list_albums` and `update_album`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/immich-google-photos-alternative](https://vinkius.com/en/ai-agent-connect/immich-google-photos-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Immich (Google Photos Alternative)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `immich-google-photos-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Immich (Google Photos Alternative)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "immich-google-photos-alternative": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
