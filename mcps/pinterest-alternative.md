# Pinterest MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pinterest-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pinterest-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pinterest-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate visual discovery via Pinterest — manage boards, create pins, and track performance directly with AI.

## Description
Connect your **Pinterest** account to any AI agent and take full control of your visual marketing and content orchestration through natural conversation. Pinterest is the world's leading visual discovery engine, and this integration allows you to retrieve board metadata, create high-impact pins, and analyze audience engagement directly from your chat interface.

### What you can do

- **Board & Profile Orchestration** — List all managed boards and retrieve detailed metadata programmatically to ensure your visual identity is always synchronized.
- **Pin Creation Intelligence** — Create new pins on specific boards with optimized titles and descriptions directly from the AI interface to drive better reach.
- **Performance & Analytics Control** — Retrieve granular analytics for individual pins and top-performing account metrics via natural language to maintain a clear overview of your visual strategy.
- **Content Discovery Oversight** — Access and monitor your board structures and pins to keep your inspiration feeds and marketing assets always optimized using simple AI commands.
- **Operational Monitoring** — Track system responses and manage user account metadata to ensure your social media workflows are always high-performing.

### How it works

1. Subscribe to this server
2. Enter your Pinterest OAuth Access Token from your developer settings
3. Start managing your visual marketing from Claude, Cursor, or any MCP-compatible client

No more manual scrolling to check pin counts or engagement. Your AI acts as a dedicated social strategist or visual content manager.

### Who is this for?

- **Digital Marketers** — quickly retrieve pin performance and monitor board growth without switching apps.
- **Content Creators** — automate the posting of new pins and track audience reach via natural conversation.
- **E-commerce Teams** — streamline the retrieval of visual assets and monitor product discovery directly within the chat.


## Available Tools
- **create_board**: Add new board
- **create_new_pin**: Required media_source must be provided as JSON.

Post new pin
- **remove_board**: Delete a board
- **remove_pin**: Delete a pin
- **get_account_performance**: Check account stats
- **get_board_info**: Get board metadata
- **get_profile_info**: Get account info
- **get_pin_performance**: Check pin stats
- **get_pin_details**: Get pin info
- **list_top_performing_pins**: List best pins
- **list_boards**: List user boards
- **list_pins_on_board**: List board pins


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pinterest** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Pinterest boards."

**🤖 AI Agent:**
> I've retrieved your boards. You have 3 active environments: 'Creative Inspiration', 'Product Catalog', and 'Marketing Assets'. Which one would you like to see pins for?

---

**👤 You:**
> "Show me my top performing pins from the last 30 days ranked by engagement."

**🤖 AI Agent:**
> Your top 5 pins by engagement this month. "Summer Home Decor Ideas" received 12,400 impressions and 847 saves (6.8% save rate). "Quick Healthy Recipes" hit 9,200 views with 623 click-throughs. "Modern Office Setup" drove 534 outbound clicks to your site. "DIY Garden Projects" generated 1,200 saves organically. "Travel Packing Guide" gained 890 repins. Total profile reach this month: 78,400 unique viewers.

---

**👤 You:**
> "Create a new pin on my Home Inspiration board with the uploaded living room image."

**🤖 AI Agent:**
> Pin created successfully on "Home Inspiration" board. Title: Modern Living Room Design. Description optimized for search with 5 relevant keywords. Link: points to your blog post. The pin is now live and discoverable. Pinterest suggests posting between 8-11 PM for this category to maximize reach. Estimated first-day impressions based on board followers: 2,400.


## Installation & Usage

To install and use the **Pinterest** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pinterest-alternative](https://vinkius.com/mcp/pinterest-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
