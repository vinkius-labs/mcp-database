# Cosmic MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cosmic)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cosmic-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cosmic-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage headless content via Cosmic — list and create objects, audit schema types, handle media assets, and manage buckets directly from any AI agent.

## Description
Connect your **Cosmic** bucket to any AI agent and take full control of your AI-powered headless CMS and digital content workflows through natural conversation.

### What you can do

- **Object Management** — List, retrieve, and create CMS objects across your buckets, allowing you to drop formatted JSON payloads feeding strictly verified metadata trees
- **Content Mutation** — Safely update existing objects by patching title and metadata blocks, substituting draft values natively through the REST API
- **Schema Auditing** — Enumerate active object types and retrieve structural extraction of properties to verify exactly what fields and metadata the schema requires
- **Media Oversight** — Inspect deep internal arrays of uploaded media, track imgix endpoints, and resolve explicit file metadata for seamless asset management
- **Bucket Cleanup** — Irreversibly vaporize explicit app nodes and wipe media assets to manage storage quotas and clear up internal database allocations
- **Environment Navigation** — Identify bounded routing spaces inside your headless environments and switch between different content models (type slugs) easily

### How it works

1. Subscribe to this server
2. Enter your Cosmic Bucket Slug and API Write Key (found in Settings > API Access)
3. Start managing your digital content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Editors** — create and update objects or manage media without navigating the Cosmic web app
- **Developers** — fetch object type schemas and verify metadata structures directly from the IDE or chat
- **Product Teams** — monitor content versioning and audit media assets across different buckets
- **Growth Teams** — quickly prototype content models and publish updates using natural language


## Available Tools
- **create_cms_object**: Provision a highly-available JSON Payload generating new Cosmic Drafts
- **wipe_media_asset**: Dispatch an automated validation check routing explicit Disk removals
- **wipe_cms_object**: Irreversibly vaporize explicit App nodes dropping live Document rows
- **get_media_asset**: Retrieve the exact structural matching verifying explicit Media IDs
- **get_single_object**: Retrieve explicit Cloud logging tracing explicit Payload IDs limitlessly
- **get_schema_details**: Perform structural extraction of properties driving active Fields
- **list_uploaded_media**: Inspect deep internal arrays mitigating specific Picture limits
- **list_schema_types**: Enumerate explicitly attached structured rules exporting active Types
- **list_bucket_objects**: Identify bounded routing spaces inside the Headless Cosmic CMS Environments
- **patch_cms_object**: Mutate global Web CRM boundaries substituting Draft values via ID


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cosmic** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all objects of type 'posts' in my Cosmic bucket"

**🤖 AI Agent:**
> I found 8 objects in the 'posts' category. The latest entries include 'AI Integration Guide' and 'Product Roadmap 2024'. Would you like to see the full metadata for any of these?

---

**👤 You:**
> "Create a new 'event' object: Title 'Developer Meetup', Date '2024-05-15'"

**🤖 AI Agent:**
> Object created! 'Developer Meetup' has been added to your bucket under the 'event' type. I've mapped the date metadata successfully. The object ID is 'abc_123'.

---

**👤 You:**
> "Show me the details for object type 'products'"

**🤖 AI Agent:**
> Retrieving schema for 'products'... This type requires fields like 'name' (text), 'price' (number), 'description' (html), and 'image' (file). I can list all the specific validation rules for you.


## Installation & Usage

To install and use the **Cosmic** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cosmic](https://vinkius.com/mcp/cosmic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
