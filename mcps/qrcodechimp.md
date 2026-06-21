# QRCodeChimp MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/qrcodechimp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Generate branded QR codes with tracking, analytics, and dynamic content that update without reprinting for any use case.

## Description
Connect your **QRCodeChimp** account to any AI agent and take full control of your digital networking and QR orchestration through natural conversation. QRCodeChimp provides a professional-grade platform for managing Digital Business Cards (DBC) and Dynamic URL QR codes in bulk, and this integration allows you to retrieve record metadata, track analytics, and manage campaigns directly from your chat interface.

### What you can do

- **Digital Business Card (DBC) Orchestration** — Find and manage professional digital profiles programmatically using short URL slugs.
- **Dynamic QR Code Control** — Create and update dynamic URL QR codes in bulk (up to 10 at a time) to ensure your physical-to-digital touchpoints are always synchronized.
- **Real-time Analytics Intelligence** — Retrieve detailed scan analytics for specific QR codes to monitor engagement and campaign performance directly from the AI interface.
- **Campaign Discovery** — List and search through your bulk QR campaigns to maintain a clear overview of your organizational assets via natural language.
- **Operational Monitoring** — Track system responses and manage QR metadata using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your QRCodeChimp API Key and API Secret from your dashboard settings
3. Start managing your digital business cards and QR codes from Claude, Cursor, or any MCP client

No more manual dashboard navigation for simple updates. Your AI acts as a dedicated asset manager or marketing coordinator.

### Who is this for?

- **Marketing Managers** — quickly retrieve scan analytics and monitor campaign reach without switching tabs.
- **Sales Operations Teams** — automate the management of digital business cards for the entire team via natural conversation.
- **Developers** — integrate dynamic QR generation and tracking into custom business workflows.


## Available Tools (11)
- **create_qrcode**: Pass QR data as a JSON string.

Create a new QR code
- **delete_qrcode**: Delete a QR code
- **get_analytics**: Get scan analytics for a QR code
- **get_bulk_qr**: Get details for a bulk QR code generation job
- **get_qrcode**: Get QR code details
- **get_scan_stats**: Get scan analytics for a QR code
- **list_campaigns**: List QR campaigns
- **list_folders**: List all QR code folders
- **list_qrcodes**: List all QR codes
- **list_templates**: List all QR code design templates
- **update_qrcode**: Update an existing QR code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **QRCodeChimp** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the digital business card with slug 'john-doe-dbc'."

**🤖 AI Agent:**
> I've retrieved the card details for 'John Doe'. It is part of the 'Corporate Team' campaign and has received 150 scans this month. Would you like to see the full analytics report?

---

**👤 You:**
> "Generate a dynamic QR code for our product catalog landing page with our brand colors and logo."

**🤖 AI Agent:**
> Dynamic QR code created (ID: qr_8234). Target URL: catalog.example.com/products. Design: Custom with brand blue (#1A5FE1) foreground, white background, company logo embedded center. Format: SVG (vector, print-ready). Scan tracking: enabled. Short URL: qrco.de/prod2025. The dynamic URL can be changed anytime without reprinting. Current scan count: 0 (just created). Download available in SVG, PNG (300dpi, 1000x1000), and PDF formats.

---

**👤 You:**
> "Show me scan analytics for all QR codes from the Spring Marketing campaign."

**🤖 AI Agent:**
> Spring Marketing campaign: 8 QR codes, 4,567 total scans this month. Top performer: "Store Window Display" with 1,890 scans (41%). "Product Packaging" at 1,234 scans. "Flyer Insert" at 678 scans. Geographic breakdown: US 62%, UK 18%, Canada 12%, Other 8%. Peak scan time: weekdays 11 AM-2 PM. Mobile OS: iOS 58%, Android 42%. Unique scanners: 3,421 (75% unique rate). Conversion to website: 67%.


## ❓ FAQ

**Q: Can my AI automatically find the details for a specific digital business card by providing its slug?**
Yes! Use the `get_qr_details` tool with the record slug (Page Code). Your agent will respond with complete metadata, including contact details and associated campaign info in seconds.

**Q: How do I find my QRCodeChimp API Key and Secret?**
Log in to your QRCodeChimp account, navigate to **Account Settings** > **API Keys Settings**, and you will find your unique API Key and Secret there.

**Q: What plan do I need for API access?**
API access typically requires a subscription to the **ULTIMA** plan or above. You may also need to contact support@qrcodechimp.com to activate the API functionality for your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/qrcodechimp](https://vinkius.com/mcp/qrcodechimp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **QRCodeChimp** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `qrcodechimp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **QRCodeChimp** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "qrcodechimp": {
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
