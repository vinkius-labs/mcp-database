# Unsplash MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/unsplash-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/unsplash-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/unsplash-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Manage your visual discovery — search photos, users, and collections via AI.

## Description
Empower your AI agent to orchestrate your entire visual ecosystem with **Unsplash**, the world's leading source of freely-usable images. By connecting Unsplash to your agent, you transform complex photo searches into a natural conversation. Your agent can instantly search for high-quality photos, audit user profiles, and retrieve curated collections without you ever touching a dashboard. Whether you are a content creator or a professional designer, your agent acts as a real-time visual curator, ensuring your projects are always powered by world-class imagery.

### What you can do

- **Photo Auditing** — Search for high-resolution images by keyword or orientation and retrieve detailed metadata, including descriptions and photographer info.
- **User Oversight** — Browse Unsplash user profiles and list all their uploaded photos to maintain a clear view of specific creators' portfolios.
- **Collection Management** — Search for and list curated collections to find themed imagery for any project instantly.
- **Visual Intelligence** — Retrieve random photos or specific photo statistics to understand image performance and reach.
- **Topic Discovery** — List curated topics on Unsplash to identify trending visual themes across the platform in real-time.

### How it works

1. Subscribe to this server
2. Enter your Unsplash Access Key (Client ID)
3. Start managing your visual assets through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Graphic Designers** — monitor image trends and retrieve specific photographer portfolios straight from your workflow.
- **Content Marketers** — verify if selected images align with brand aesthetic and retrieve high-quality alternatives.
- **Art Directors** — perform rapid audits of curated collections and identify new visual themes without manual logins.
- **Operations Leads** — automate visual data querying to orchestrate cross-functional creative teams smoothly.


## Available Tools
- **get_collection**: Get details for a specific collection
- **get_photo_stats**: Get statistics for a specific photo
- **get_photo**: Get details for a specific photo
- **get_random_photo**: Get a random high-quality photo
- **get_user_photos**: Get photos uploaded by a specific user
- **get_user**: Get details for a specific user
- **list_topics**: List curated topics on Unsplash
- **search_collections**: Search for curated collections on Unsplash
- **search_photos**: Search for high-quality photos on Unsplash
- **search_users**: Search for users on Unsplash


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Unsplash** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for landscape photos of 'Alpine mountains' on Unsplash."

**🤖 AI Agent:**
> I've retrieved high-quality landscape photos of Alpine mountains. Top matches include images by several professional photographers. Would you like the direct links to download them?

---

**👤 You:**
> "Get a random photo about 'Cyberpunk city'."

**🤖 AI Agent:**
> Random photo selected! I've found a stunning image of a neon-lit urban landscape. The photographer is 'John Doe' and you can access the full resolution via the provided URL.

---

**👤 You:**
> "List photos from user 'vinkius_creative'."

**🤖 AI Agent:**
> I've found 10 uploads from 'vinkius_creative'. The portfolio includes diverse themes like 'Nature' and 'Tech'. Would you like the metadata for the most recent upload?


## Installation & Usage

To install and use the **Unsplash** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/unsplash-alternative](https://vinkius.com/mcp/unsplash-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
