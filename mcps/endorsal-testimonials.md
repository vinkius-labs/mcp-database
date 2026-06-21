# Endorsal Testimonials MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/endorsal-testimonials)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/endorsal-testimonials-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/endorsal-testimonials-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Equip your AI agent to manage testimonials, track display widgets, and approve reviews via the Endorsal API.

## Description
Integrate **Endorsal**, the fully automated testimonial collection platform, directly into your AI workflow. Manage your collected testimonials and customer ratings, track display widgets and website properties, monitor pending reviews and approval statuses, and oversee your social proof using natural language.

### What you can do

- **Testimonial Oversight** — List and retrieve detailed content, customer ratings, and photos for all your collected testimonials.
- **Widget Intelligence** — Monitor display widgets and properties, resolving widget types and deployment identifiers across your brands.
- **Approval Management** — Access and approve pending testimonials, ensuring high-quality social proof is published instantly.
- **Social Proof Auditing** — Retrieve high-level summaries of review volumes, widget activity, and organizational social proof health instantly.

### How it works

1. Connect the Endorsal integration to your AI assistant.
2. Authorize using your Endorsal API Key (found in your account settings).
3. Orchestrate your social proof strategy and review management through intuitive conversation.

### Who is this for?

- **Marketing Managers** — Quickly check recent testimonial ratings and approval queues on the go.
- **Content Creators** — Research customer quotes and social proof snippets via chat for marketing copy.
- **Operations Teams** — Monitor review volumes and organizational Endorsal metadata instantly.


## Available Tools
- **quick_social_proof_audit**: Retrieve a high-level summary of testimonials and widget activity
- **approve_pending_testimonial**: Approve a pending testimonial for public display
- **get_endorsal_account_metadata**: Retrieve metadata and limits for your Endorsal account
- **get_testimonial_details**: Get full content and metadata for a specific testimonial
- **list_pending_testimonials**: Identify testimonials that are currently awaiting approval
- **list_account_properties**: List all properties (websites/brands) managed in your account
- **list_latest_testimonials**: Identify the most recently collected testimonials
- **list_all_testimonials**: List all testimonials collected in your Endorsal account
- **list_display_widgets**: g. wall of love, badge), and unique identifiers.

List all display widgets configured in your account
- **search_testimonials_by_keyword**: Search for testimonials using a customer name or testimonial keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Endorsal Testimonials** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my collected testimonials."

**🤖 AI Agent:**
> I've found 15 testimonials, including 'Excellent Service' (5 stars) and 'Highly Recommended' (5 stars). 12 are approved and 3 are pending. Would you like to see the text for the pending ones?

---

**👤 You:**
> "Show me the display widgets configured."

**🤖 AI Agent:**
> I've retrieved 4 widgets, including 'Main Website Wall' (Wall of Love), 'Sidebar Badge', and 'Checkout Slider'. Should I pull the specific property ID for the Main Website Wall?

---

**👤 You:**
> "Approve testimonial ID 'TEST-12345'."

**🤖 AI Agent:**
> Testimonial ID 'TEST-12345' from 'John Doe' has been successfully approved and is now live on your configured widgets. Should I notify the team?


## Installation & Usage

To install and use the **Endorsal Testimonials** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/endorsal-testimonials](https://vinkius.com/mcp/endorsal-testimonials)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
