# Imagine.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/imagineio)
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


## Available Tools (10)
- **get_product**: Get product details
- **get_scene**: Get scene details
- **list_materials**: List available materials
- **list_products**: io account with their render status and metadata.

List all 3D products
- **list_renders**: List product renders
- **list_scenes**: List all scenes
- **check_imagine_status**: Verify Imagine API connectivity
- **create_render_job**: The job runs asynchronously; check status with get_job_status.

Start a 3D render job
- **get_account**: io account details and render credit balance.

Get account info
- **get_job_status**: Check render job status


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


## ❓ FAQ

**Q: How do I start a 3D render job?**
Use the `create_render_job` tool with a product identifier. The render runs asynchronously — check progress with `get_job_status`.

**Q: Can I browse available 3D scenes and materials?**
Yes. Use `list_scenes` to browse environments and `list_materials` to see all available textures and finishes for your products.

**Q: How do I download the final rendered images?**
Use `list_renders` with the product identifier to retrieve all completed render URLs including resolution details and download links.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/imagineio](https://vinkius.com/mcp/imagineio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Imagine.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `imagineio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Imagine.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "imagineio": {
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
