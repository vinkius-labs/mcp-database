# Imagine.io MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/imagineio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/imagineio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/imagineio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Create 3D product visualizations and room renders from photos using AI that turns concepts into photorealistic images.

## Description
Connect your **Imagine.io** account to any AI agent and take full control of your 3D product visualization and automated content generation workflows through natural conversation.

### What you can do

- **Project & Product Orchestration** â€” List and manage your entire portfolio of 3D products programmatically, retrieving detailed technical metadata and SKU IDs
- **Content Job Intelligence** â€” Programmatically trigger and monitor 3D generation jobs (Viewer, AR, 360Â° Spin) to maintain a perfectly coordinated output pipeline
- **Asset Architecture Monitoring** â€” Access real-time statuses for 3D processing and retrieve hosted asset URLs (Viewer URLs, images) directly through your agent
- **Shared Content Discovery** â€” Access generated outputs and their metadata directly through your agent for instant operational reporting
- **Operational Monitoring** â€” Verify account-level API connectivity and monitor content generation volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** and **Registered Domain** from your Imagine.io dashboard (Settings > API Access)
3. Start orchestrating your 3D assets from Claude, Cursor, or any MCP client

No more manual checking of individual job statuses or missing 3D viewer links. Your AI acts as your dedicated 3D coordinator and asset architect.

### Who is this for?

- **E-commerce Managers** â€” instantly retrieve 3D viewer links and monitor content job status using natural language commands
- **3D Artists & Developers** â€” verify asset metadata and track processing health without leaving your creative workspace
- **Operations Leads** â€” automate the management of 3D product portfolios through simple AI queries


## Available Tools
- **check_imagine_status**: Verify Imagine API connectivity
- **create_render_job**: The job runs asynchronously; check status with get_job_status.

Start a 3D render job
- **get_account**: io account details and render credit balance.

Get account info
- **get_job_status**: Check render job status
- **get_product**: Get product details
- **get_scene**: Get scene details
- **list_materials**: List available materials
- **list_products**: io account with their render status and metadata.

List all 3D products
- **list_renders**: List product renders
- **list_scenes**: List all scenes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Imagine.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my 3D products in Imagine."

**🤖 AI Agent:**
> You have 12 products in your account. The most recent is 'White Sneaker v2' with 3 completed renders. Would you like to start a new render or view details?

---

**👤 You:**
> "Start a render for product 'PROD-4821'."

**🤖 AI Agent:**
> Render job submitted for PROD-4821. Job ID: JOB-9173. Estimated time: 4 minutes. I'll check the status for you — would you like me to notify you when it's done?

---

**👤 You:**
> "Show me all scenes available for product placement."

**🤖 AI Agent:**
> You have 8 scenes available: 'Studio White', 'Kitchen Modern', 'Living Room Warm', and 5 more. Each scene includes customizable lighting and camera angles. Want to see details for any of them?


## Installation & Usage

To install and use the **Imagine.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/imagineio](https://vinkius.com/mcp/imagineio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
