# Flowcode MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flowcode)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage dynamic QR codes, track scan analytics, and oversee Flowpages via AI agents with Flowcode.

## Description
Connect your **Flowcode** account to any AI agent and automate your offline-to-online marketing through the Model Context Protocol (MCP). Flowcode is the leading platform for dynamic QR codes and conversion-optimized landing pages (Flowpages). Now, you can create new codes, monitor scan performance, and retrieve deep audience analytics directly through natural conversation.

### What you can do

- **Dynamic QR Management** — List all your Flowcodes, fetch detailed metadata, and create new dynamic codes with instant redirect capabilities.
- **Scan Analytics** — Monitor real-time scan performance, conversion rates, and detailed scan activity logs to optimize your campaigns.
- **Flowpage Oversight** — Retrieve real-time event data for your landing pages and access CRM contact information submitted via Flowpage forms.
- **Audience Insights** — Fetch aggregate demographic and geographic analytics to understand where and how your audience is engaging.
- **Asset Organization** — List campaigns and asset folders to maintain a clear structure across your marketing projects.
- **Image Generation** — Retrieve specific Flowcode image data or download links directly from the agent.
- **Custom Conversions** — Track conversion rates from scan to visit to ensure your marketing funnel is performing optimally.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Flowcode API Key (found in your Flowcode Developer Portal)
3. Start managing your dynamic QR codes and analytics from Claude, Cursor, or any MCP client

### Who is this for?

- **Marketing Managers** — quickly create a new QR code for a print campaign or check scan stats before a meeting.
- **Brand Operations** — get a real-time overview of geographic engagement across all active Flowcodes through simple AI commands.
- **Sales Teams** — automate the retrieval of lead contact info submitted through offline QR code interactions.


## Available Tools
- **create_flowcode**: Create a dynamic QR code
- **get_flowpage_contacts**: Get CRM contacts
- **get_audience_summary**: Get audience demographics
- **get_flowcode_image**: Generate QR code image
- **get_flowcode**: Get Flowcode details
- **get_flowpage_analytics**: Get landing page events
- **get_geographic_analytics**: Get scan locations
- **get_recent_scans**: List scan activity log
- **list_campaigns**: List marketing campaigns
- **list_conversion_rates**: Get funnel analytics
- **list_flowcodes**: List all Flowcodes
- **list_folders**: List asset folders


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flowcode** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my 10 most recent Flowcodes and their scan counts."

**🤖 AI Agent:**
> Fetching Flowcodes... I found your 10 most recent dynamic QR codes, including 'Fall Campaign' (1,250 scans) and 'Product Demo' (450 scans). Would you like to see the geo-analytics for any of these?

---

**👤 You:**
> "Create a new Flowcode named 'Store Launch' redirecting to 'https://vinkius.com'."

**🤖 AI Agent:**
> Flowcode created! I've generated a new dynamic QR code named 'Store Launch' pointing to vinkius.com. The code ID is 'code_123'. I can provide the image download link whenever you're ready.

---

**👤 You:**
> "Show me the audience demographic summary for my account."

**🤖 AI Agent:**
> Retrieving audience data... Your engagement is primarily coming from users aged 25-34 (45%) using mobile devices. The top scan locations are New York and London. Would you like a more detailed breakdown?


## ❓ FAQ

**Q: Can I change the destination URL of a Flowcode after it has been created?**
Yes! Flowcodes are dynamic by default. You can use the 'create_flowcode' or future update tools via the agent to manage your redirect rules without needing to change the physical QR code image.

**Q: How do I see where my QR codes are being scanned geographically?**
You can use the 'get_geographic_analytics' tool. The agent will retrieve a summary of scan distribution across different regions, helping you understand where your offline audience is most active.

**Q: Can I retrieve contact info from users who scanned my codes?**
Yes! If you have forms on your Flowpages, you can use the 'get_flowpage_contacts' tool to retrieve submissions, including names and emails, directly through the agent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flowcode](https://vinkius.com/mcp/flowcode)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flowcode** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `flowcode` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flowcode** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flowcode": {
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
