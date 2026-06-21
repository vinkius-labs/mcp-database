# Snapchat Conversions MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/snapchat-conversions)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/snapchat-conversions-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/snapchat-conversions-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Send conversion events to Snapchat Ads via the Conversions API with AI agents.

## Description
Connect your **Snapchat Ads** account to any AI agent to automate your server-side conversion tracking and marketing attribution. Snapchat Conversions API (CAPI) provides a robust platform for reporting web and app events, and this integration allows you to send conversion metadata, track purchases, and monitor sign-ups through natural conversation.

### What you can do

- **Event Reporting Orchestration** — Send real-time conversion events (Purchase, Page View, Sign Up) programmatically to optimize your Snapchat ad performance.
- **User Data Management** — Submit hashed customer metadata to ensure high match rates and accurate attribution directly from the AI interface.
- **App Event Integration** — Report app-specific events like App Open or In-App Purchases to track your mobile campaign ROI via natural language.
- **Compliance & Hashing Monitoring** — Access integration guidelines to ensure all PII is properly SHA-256 hashed before transmission.
- **Operational Monitoring** — Track event submission results and monitor API health to ensure your marketing data is always synchronized.

### How it works

1. Subscribe to this server
2. Enter your Snapchat Conversions API Token from Ads Manager
3. Start managing your marketing attributions from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Performance Marketers** — quickly report offline or server-side conversions and monitor ad attribution without switching apps.
- **Growth Engineers** — automate the sending of custom conversion events and monitor event match quality via natural conversation.
- **Operations Teams** — streamline the retrieval of integration guidelines and monitor marketing data flow directly within the chat.


## Available Tools
- **check_capi_health**: Verify CAPI status
- **get_capi_integration_guidelines**: Get best practices for hashing
- **list_supported_conversion_events**: List valid event types
- **track_add_to_cart_event**: Track an item added to cart
- **track_app_open_event**: Track a mobile app opening
- **track_page_view_event**: Track a website page view
- **track_purchase_event**: Requires pixel_id and user identifiers.

Track a successful purchase
- **send_custom_conversion_event**: Send a raw JSON conversion event
- **track_search_event**: Track a site search
- **track_sign_up_event**: Track a new user registration
- **track_start_checkout_event**: Track the start of checkout
- **track_view_content_event**: Track a product detail view


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Snapchat Conversions** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a PURCHASE conversion event to Snapchat with pixel ID 'abc-123'."

**🤖 AI Agent:**
> Conversion event triggered! I've successfully reported the purchase event to Snapchat via the Conversions API. Transaction ID: TXN-456.

---

**👤 You:**
> "Show me the conversion funnel performance for all active Snapchat ad campaigns."

**🤖 AI Agent:**
> 4 active Snapchat campaigns. "Summer Collection" (swipe-up): 234K impressions, 12.4K swipes (5.3% CTR), 890 add-to-carts, 234 purchases. ROAS: 4.2x. Spend: $2,340. Revenue: $9,828. "App Install" (deep link): 156K impressions, 8.9K taps, 2,340 installs. CPI: $1.23. "Brand Awareness" (story ad): 890K impressions, 67K views (7.5% VTR). "Lead Gen" (form): 45K impressions, 1,200 leads. CPL: $3.80. Total Snap Pixel events tracked: 45,678.

---

**👤 You:**
> "Send a batch of purchase conversion events for orders processed through our checkout today."

**🤖 AI Agent:**
> Conversion events batch sent to Snapchat Conversions API. Events: 67 PURCHASE events. Total revenue reported: $8,945. Average order value: $133.51. Deduplication: 4 events matched existing Snap Pixel events (removed). Net new: 63 events. Match rate: 89% (Snapchat matched 56 events to Snapchat users). Attribution window: 28-day click, 1-day view. Events timestamped with original transaction time. Next sync scheduled: 6 hours. Campaign optimization data will update within 4 hours.


## Installation & Usage

To install and use the **Snapchat Conversions** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/snapchat-conversions](https://vinkius.com/mcp/snapchat-conversions)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
