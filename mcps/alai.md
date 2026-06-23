# Alai MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/alai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Generate professional headshots and profile photos with AI that transforms selfies into studio-quality business portraits.

## Description
Connect your **Alai** (getalai.com) account to any AI agent and take full control of your automated marketing content generation and high-fidelity asset distribution through natural conversation.

### What you can do

- **Content Portfolio Orchestration** — List and manage your entire high-fidelity portfolio of AI-generated marketing assets programmatically, retrieving detailed platform metadata
- **Campaign & Request Intelligence** — Programmatically trigger and monitor real-time content generation jobs to maintain a perfectly coordinated marketing pipeline
- **Asset Monitoring Discovery** — Access real-time status updates for processed assets (images, text) and track individual performance metrics directly through your agent
- **Metadata Management** — Programmatically retrieve high-fidelity content IDs and session status to maintain a perfectly coordinated media record
- **Operational Monitoring** — Verify account-level API connectivity and monitor orchestration volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Alai dashboard (Settings > API)
3. Start orchestrating your marketing growth from Claude, Cursor, or any MCP client

No more manual creation of individual marketing posts or missing critical generation status. Your AI acts as your dedicated content coordinator and marketing architect.

### Who is this for?

- **Marketing Managers** — instantly retrieve asset performance recaps and monitor content generation using natural language commands
- **Growth Leads** — verify individual asset metadata and track creation history without leaving your creative workspace
- **Developers** — integrate high-speed Alai marketing data into custom CRM and social media pipelines through simple AI queries


## Available Tools (12)
- **check_getalai_status**: Verify connectivity
- **create_asset**: Create an asset
- **create_campaign**: Create a campaign
- **delete_asset**: Delete an asset
- **generate_content**: Generate AI content
- **get_asset**: Get asset details
- **get_campaign**: Get campaign details
- **get_generation**: Get generation details
- **list_assets**: List assets
- **list_campaigns**: List campaigns
- **list_generations**: List generations
- **list_templates**: List templates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Alai** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active marketing campaigns in my Alai account."

**🤖 AI Agent:**
> I've retrieved your campaigns. You currently have 5 active high-fidelity profiles, including 'Social Media Push' and 'Email Blast B'. Would you like the detailed platform metadata for any of them?

---

**👤 You:**
> "Show the last 5 assets generated for 'Social Media Push'."

**🤖 AI Agent:**
> Asset directory orchestrated! For 'Social Media Push', I've identified 5 recent high-fidelity assets, including 3 images and 2 text posts. I've retrieved the technical creation metadata for your review. Need help retrieving the final hosted URLs?

---

**👤 You:**
> "Check for any content generation jobs in 'Processing' status."

**🤖 AI Agent:**
> Operational monitoring orchestrated! I've identified 2 high-fidelity jobs currently in 'Processing' status, including 'Banner A' and 'Blog Post B'. Your API connection is healthy. Shall I notify you once these assets are ready for distribution?


## ❓ FAQ

**Q: How do I find my Alai API Key?**
Log in to your account, navigate to **Settings** > **API**, and copy your unique access token from the credentials section.

**Q: Can I retrieve generated assets via AI?**
Yes! The `list_alai_assets` tool allows your agent to retrieve high-fidelity metadata and hosted URLs for all your AI-generated content.

**Q: How do I list my active campaigns?**
Use the `list_alai_campaigns` tool to retrieve your complete high-fidelity directory along with the unique identifiers for all managed marketing workstreams.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/alai](https://vinkius.com/mcp/alai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Alai** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `alai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Alai** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "alai": {
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
