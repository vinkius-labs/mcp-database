# Sharpei MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sharpei)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sharpei-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sharpei-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **Sharpei** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sharpei](https://vinkius.com/mcp/sharpei)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
