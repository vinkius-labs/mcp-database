# Apple App Store MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/apple-app-store)
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


## Available Tools (8)
- **get_account_check**: Verify App Store Connect account connection
- **get_sales_reports**: frequency can be DAILY, WEEKLY, MONTHLY, or YEARLY.

Download sales and trends reports
- **list_apps**: List all apps in your App Store Connect account
- **list_builds**: List all builds for an app
- **list_customer_reviews**: List customer reviews for an app
- **get_app_info**: Get details for a specific app
- **get_app_store_versions**: List all App Store versions for an app
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


## ❓ FAQ

**Q: How do I create an App Store Connect API Key?**
Log in to App Store Connect, go to **Users and Access**, select the **Integrations** tab, and then **App Store Connect API**. You can generate and download your private key (.p8) there.

**Q: What is my Issuer ID and Key ID?**
The Issuer ID is a unique ID for your organization, and the Key ID is specific to the API key you generated. Both are displayed on the App Store Connect API keys page.

**Q: How are sales reports handled?**
The `get_sales_reports` tool initiates a download of aggregated sales data from Apple. Note that detailed reports are provided as compressed files which are processed by the server.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apple-app-store](https://vinkius.com/mcp/apple-app-store)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Apple App Store** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `apple-app-store` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Apple App Store** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "apple-app-store": {
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
