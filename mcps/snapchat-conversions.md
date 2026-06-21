# Snapchat Conversions MCP Server

Send conversion events to Snapchat Ads via the Conversions API with AI agents.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/snapchat-conversions)

## Overview
**Category:** industry-titans
**Tools Count:** 12

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


## Installation & Usage

To install and use the **Snapchat Conversions** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/snapchat-conversions](https://vinkius.com/mcp/snapchat-conversions)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
