# Design Pickle MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/design-pickle)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to manage graphic design requests, track brand profiles, and monitor your production queue via the Design Pickle API.

## Description
Integrate **Design Pickle**, the world's leading unlimited graphic design service, directly into your AI workflow. Manage your creative projects, audit your brand guidelines and profiles, and track the status of your design queue using natural language.

### What you can do

- **Request Management** — List and retrieve detailed information for all your design requests and their current production status.
- **Brand Identity Oversight** — Access your brand profiles, including logos, color palettes, and typography guidelines.
- **Queue Monitoring** — Track your production pipeline and stay informed on estimated delivery timelines.
- **Asset Retrieval** — List and access files and delivered designs for your active and past requests.

### How it works

1. Connect the Design Pickle integration to your AI assistant.
2. Authorize using your Design Pickle API Key (found in your account settings).
3. Orchestrate your creative workflow and brand management through intuitive conversation.

### Who is this for?

- **Marketing Managers** — Quickly check the status of active design requests and production timelines on the go.
- **Creative Directors** — Audit brand profiles and guidelines to ensure consistency across projects via chat.
- **Small Business Owners** — Manage their design queue and access delivered assets effortlessly.


## Available Tools (10)
- **get_account_metadata**: Retrieve metadata and settings for your Design Pickle account
- **get_brand_profile_details**: Get full details for a specific brand profile
- **get_production_queue_status**: Check the current status of your production queue
- **get_design_request_details**: Get detailed information for a specific design request
- **list_brand_profiles**: List all brand profiles configured for your designs
- **list_recently_delivered_designs**: Identify design requests that have been recently completed and delivered
- **list_assigned_designers**: List designers currently assigned to your account
- **list_design_requests**: g., in progress, delivered), and designer assignments.

List all graphic design requests in your Design Pickle account
- **list_active_subscriptions**: List active Design Pickle service plans and subscriptions
- **search_design_requests**: Search for design requests using a keyword in the title


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Design Pickle** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my design requests currently in progress."

**🤖 AI Agent:**
> I've found 3 design requests in progress: 'Social Media Banner Set', 'Q3 Presentation Deck', and 'New Product Logo'. Would you like to see the estimated delivery time for any of these?

---

**👤 You:**
> "Show me our brand profile guidelines for 'Main Brand'."

**🤖 AI Agent:**
> I've retrieved the 'Main Brand' profile. It includes your primary logo (Main_Logo.png), color palette (#3498db, #2ecc71, #f1c40f), and typography settings (Open Sans, Roboto). Should I check if these guidelines are applied to your recent requests?

---

**👤 You:**
> "What is the status of our production queue?"

**🤖 AI Agent:**
> Your production queue currently has 5 active requests. 2 are being worked on by your assigned designers, and 3 are in the triage phase. The next delivery is expected within 24 hours. Would you like a detailed breakdown?


## ❓ FAQ

**Q: How do I get a Design Pickle API Key?**
Log in to your Design Pickle account, navigate to your settings or API section, and you can generate or retrieve your unique API Key from there.

**Q: Can the agent see my designers?**
Yes, you can use the list_assigned_designers tool to see the creative team members associated with your account.

**Q: Does the integration show real-time production status?**
Yes, you can check the production queue status and individual request details to see where your designs are in the creative process.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/design-pickle](https://vinkius.com/mcp/design-pickle)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Design Pickle** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `design-pickle` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Design Pickle** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "design-pickle": {
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
