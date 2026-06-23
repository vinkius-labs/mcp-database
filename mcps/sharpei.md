# Sharpei MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sharpei)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Offer product subscriptions and rentals on your Shopify store with flexible recurring payment options your customers will love.

## Description
Connect your **Sharpei** account to any AI agent and manage identity verification workflows through natural conversation.

### What you can do

- **Application Management** — List, inspect, and create verification applications
- **Document Review** — View uploaded documents and check verification results
- **Status Tracking** — Monitor verification progress for each application
- **Subscription Management** — View plans and features
- **Webhook Configuration** — List configured webhook endpoints


## Available Tools (10)
- **check_sharpei_status**: Verify API connectivity
- **create_application**: Create a verification application
- **get_application**: Get application details
- **get_document**: Get document details
- **get_documents**: List application documents
- **get_subscription**: Get subscription details
- **get_verification_status**: Get verification status
- **list_applications**: List all applications
- **list_subscriptions**: List subscriptions
- **list_webhooks**: List webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sharpei** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all verification applications."

**🤖 AI Agent:**
> You have 15 applications: 8 approved, 4 pending, 3 under review. The most recent is APP-2891 (John D., submitted today).

---

**👤 You:**
> "Check verification status for application APP-2891."

**🤖 AI Agent:**
> Application APP-2891 is 'Under Review'. 2 of 3 documents verified successfully. Passport is pending manual review.

---

**👤 You:**
> "Create a verification application for Jane Smith, jane@example.com."

**🤖 AI Agent:**
> Application created! ID: APP-2892 for Jane Smith. Next step: the customer needs to upload identity documents.


## ❓ FAQ

**Q: Can my AI create a new verification application?**
Yes. Use `create_application` with the customer name and email. The agent starts the verification process and returns the application ID.

**Q: How do I check document verification results?**
Use `get_document` with the application and document IDs. The agent returns verification status, document type, and any flags.

**Q: Can I track the overall verification status?**
Yes. `get_verification_status` returns the current status of any application — pending, approved, or rejected.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sharpei](https://vinkius.com/mcp/sharpei)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sharpei** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sharpei` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sharpei** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sharpei": {
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
