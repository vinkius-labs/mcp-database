# Elastic Path MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/elastic-path)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/elastic-path-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/elastic-path-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage headless commerce workflows via Elastic Path — inspect carts, track purchases, and retrieve store navigation directly from any AI agent.

## Description
Connect your **Elastic Path** commerce engine to any AI agent to streamline your headless commerce operations through natural language.

### What you can do

- **Cart & Profile Management** — Access default carts and user profiles for specific store scopes to understand customer context.
- **Order Tracking** — Retrieve detailed purchase information, including status (COMPLETE/FAILED), totals, and line items using specific IDs.
- **Store Discovery** — Fetch navigation entry points, search configurations, and supported country lists for your storefront.
- **Account Services** — Access registration forms and account-specific metadata to manage user lifecycles.
- **Deep Data Inspection** — Use zoom and format parameters to retrieve linked data and specific response formats directly from the Cortex API.

### How it works

1. Subscribe to this server
2. Enter your Elastic Path Cortex URL and Access Token
3. Start managing your commerce workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — quickly check order statuses and store configurations without logging into multiple dashboards.
- **Developers** — test API responses and inspect cart/navigation structures directly from the code editor.
- **Support Teams** — retrieve account and purchase details instantly to resolve customer inquiries faster.


## Available Tools
- **create_token**: Authenticate and create an OAuth2 token
- **get_account**: Read a specific account
- **get_countries**: Get geographies/countries for a scope
- **get_default_cart**: Read the default cart for a scope
- **get_default_profile**: Read the default profile for a scope
- **get_navigations**: Get navigations entry point for a scope
- **get_purchase**: Returns status (COMPLETE, FAILED), totals, and line items.

Read a specific purchase
- **get_registration_form**: Get account registration form for a scope
- **get_searches**: Get searches entry point for a scope


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Elastic Path** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the default cart for the 'mobee' scope."

**🤖 AI Agent:**
> I've retrieved the default cart for 'mobee'. It currently contains 3 items with a total value of $145.00. Would you like to see the specific line items?

---

**👤 You:**
> "What is the status of purchase ID '12345' in the 'mobee' scope?"

**🤖 AI Agent:**
> The purchase '12345' is marked as 'COMPLETE'. The transaction was finalized on Oct 24th for a total of $89.99.

---

**👤 You:**
> "List the available countries for our store scope."

**🤖 AI Agent:**
> I've fetched the supported geographies. Your store currently supports shipping and billing in 5 countries: USA, Canada, UK, Germany, and France.


## Installation & Usage

To install and use the **Elastic Path** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/elastic-path](https://vinkius.com/mcp/elastic-path)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
