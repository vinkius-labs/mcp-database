# Apple App Store MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apple-app-store)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/apple-app-store-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/apple-app-store-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your iOS apps and TestFlight builds with Apple App Store Connect — track reviews, versions, and sales via AI.

## Description
The **Apple App Store MCP Server** provides a direct natural language interface to your App Store Connect account. Empower your AI agent to monitor your app's health, manage TestFlight builds, and analyze customer feedback without ever leaving your workflow.

### Key Capabilities

- **App Inventory** — List all apps in your account and get detailed metadata for any specific product.
- **Customer Reviews** — Access and analyze customer feedback and star ratings across all territories.
- **Version History** — Track your App Store versions, release notes, and current submission statuses.
- **TestFlight & Builds** — Monitor your latest builds and prerelease versions for beta testing.
- **Sales & Trends** — Download aggregated sales reports to track downloads and revenue performance.
- **Account Oversight** — Quickly verify your connection and account status using secure JWT authentication.

### Who is this for?

- **iOS Developers** — Keep track of build statuses and TestFlight updates using simple natural language commands.
- **Product Managers** — Quickly gather user feedback and version history for performance reviews and planning.
- **Marketing Teams** — Monitor App Store metadata and sales trends to optimize store presence and measure campaign success.


## Available Tools
- **get_account_check**: Verify App Store Connect account connection
- **get_app_info**: Get details for a specific app
- **get_app_store_versions**: List all App Store versions for an app
- **get_sales_reports**: frequency can be DAILY, WEEKLY, MONTHLY, or YEARLY.

Download sales and trends reports
- **list_apps**: List all apps in your App Store Connect account
- **list_builds**: List all builds for an app
- **list_customer_reviews**: List customer reviews for an app
- **list_prerelease_versions**: List prerelease (TestFlight) versions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Apple App Store** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my apps in App Store Connect."

**🤖 AI Agent:**
> I've retrieved your apps. You have 3 apps: 'Fitness Tracker', 'Recipe Master', and 'Expense Guide'.

---

**👤 You:**
> "What is the status of my latest build for 'Fitness Tracker'?"

**🤖 AI Agent:**
> The latest build (version 2.1.0, build 45) for 'Fitness Tracker' is currently 'Ready for Testing' in TestFlight.

---

**👤 You:**
> "Show me recent reviews for appId '123456789'."

**🤖 AI Agent:**
> I've found 5 new reviews for your app. The average rating is 4.5 stars, with users praising the new UI layout.


## Installation & Usage

To install and use the **Apple App Store** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apple-app-store](https://vinkius.com/mcp/apple-app-store)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
