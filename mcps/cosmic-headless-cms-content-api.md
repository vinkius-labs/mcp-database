# Cosmic (Headless CMS & Content API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cosmic-headless-cms-content-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your content, media, and object types via Cosmic — list objects, create content, and handle media assets directly through any AI agent.

## Description
Connect your **Cosmic** headless CMS to any AI agent to manage your content infrastructure through natural language. Cosmic provides a powerful API-first approach to content management, and this MCP server brings those capabilities directly to your AI workflows.

### What you can do

- **Content Management** — Create, read, update, and delete objects across your buckets with full metadata support.
- **Media Library** — List, upload, and manage your media assets including images, videos, and documents.
- **Schema Control** — Manage object types and structures programmatically to maintain your content model.
- **Version Control** — Access and manage revisions to track changes and restore previous versions of your content.
- **Batch Operations** — Execute multiple object operations in a single request for high-efficiency updates.

### How it works

1. Subscribe to this server
2. Provide your Cosmic Bucket Slug, Read Key, and Write Key
3. Start managing your headless CMS from Claude, Cursor, or any MCP client

### Who is this for?

- **Developers** — Quickly query content structures or update metadata without leaving the code editor.
- **Content Managers** — Use AI to draft new objects, organize media, or audit existing content entries.
- **Product Teams** — Automate content updates and maintain consistency across multiple buckets.


## Available Tools (21)
- **delete_object_type**: Specify both the slug and the bucket slug.

Delete an Object Type
- **create_object**: Specify the object type and the target bucket slug.

Create a new Object
- **delete_media**: Provide both the media ID and the bucket slug.

Delete Media
- **list_agent_conversations**: Supply the agent ID.

List conversations for an AI Agent
- **list_revisions**: Supply the object ID and bucket slug.

Get Revisions for an Object
- **batch_objects**: Limit operations to a maximum of 25.

Perform batch operations on Objects (Max 25)
- **create_media**: Specify the target bucket slug for the media payload.

Create/Upload Media
- **create_object_type**: Specify the bucket slug where the type belongs.

Create a new Object Type
- **create_revision**: Supply the object ID, bucket slug, and the revision body.

Add a Revision for an Object
- **delete_object**: Provide both the object ID and the bucket slug.

Delete an Object
- **get_agent_conversation_history**: Pass the agent ID and conversation ID.

Get history for a specific Agent conversation
- **get_object**: Provide the bucket slug if the object is not in the default bucket.

Get a single Object by ID
- **get_object_type**: Provide the slug and the bucket slug.

Get a single Object Type by slug
- **get_revision**: Provide the object ID, revision ID, and bucket slug.

Get a single Revision for an Object
- **list_media**: Use the query parameter to filter results.

List Media in a Cosmic Bucket
- **list_object_types**: Specify the bucket slug.

List Object Types in a Cosmic Bucket
- **list_objects**: Use the query parameter (URL encoded JSON) to filter results.

List Objects in a Cosmic Bucket
- **send_agent_message**: Provide the agent ID and the message content.

Send a message to an AI Agent
- **update_media**: Provide the media ID and the bucket slug.

Update Media metadata
- **update_object**: Supply the object ID and the bucket slug for accurate targeting.

Update an existing Object
- **update_object_type**: Provide the slug and ensure the object type exists.

Update an Object Type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cosmic (Headless CMS & Content API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 objects of type 'news' in my bucket."

**🤖 AI Agent:**
> I've retrieved the latest 'news' objects. Here are the most recent entries: 'Product Launch' (ID: abc1), 'New Partnership' (ID: abc2), and 3 others. Would you like to see the full content of any of these?

---

**👤 You:**
> "Create a new draft post titled 'AI and CMS' with the type 'blog-posts'."

**🤖 AI Agent:**
> Successfully created the draft object 'AI and CMS' (ID: xyz789) in the 'blog-posts' category. You can now add metadata or publish it when ready.

---

**👤 You:**
> "Show me all media files currently in the bucket."

**🤖 AI Agent:**
> I found 12 media assets in your bucket. Recent uploads include 'hero-banner.jpg', 'logo-white.png', and 'intro-video.mp4'. Do you need the URL for any specific file?


## ❓ FAQ

**Q: Can I filter objects by a specific type like 'blog-posts'?**
Yes! Use the `list_objects` tool and provide a JSON query string like `{"type":"blog-posts"}` in the query parameter to filter your results.

**Q: How do I update the content of an existing object?**
You can use the `update_object` tool. Provide the Object ID and the new values for `title`, `metadata`, or `status` to modify the entry.

**Q: Is it possible to see who made changes to an object?**
Yes, you can use the `list_revisions` tool for a specific object to see its history, and `get_revision` to inspect the details of a specific version.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cosmic-headless-cms-content-api](https://vinkius.com/en/ai-agent-connect/cosmic-headless-cms-content-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cosmic (Headless CMS & Content API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cosmic-headless-cms-content-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cosmic (Headless CMS & Content API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cosmic-headless-cms-content-api": {
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
