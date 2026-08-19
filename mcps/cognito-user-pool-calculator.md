# Cognito User Pool Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/cognito-user-pool-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Estimate AWS Cognito resource usage, limits, and token profiles.

## Description
Plan your AWS Cognito architecture with precision. This MCP server provides deterministic calculations for user pool capacity, security profiles, and resource usage. Use `calculate_pool_capacity` to check if your user, app client, or identity provider counts fit within recommended limits. Use `estimate_security_profile` to determine JWT token sizes and validate password policies. You can also use `calculate_resource_usage` to monitor custom attributes and Lambda triggers, or `estimate_sms_throughput` to predict daily messaging limits.


## Available Tools (4)
- **estimate_security_profile**: Estimate the data footprint and security configuration of the authentication flow
- **estimate_sms_throughput**: Estimate daily messaging limits for the configured user base
- **calculate_pool_capacity**: Calculate how many resources will fit within a single Cognito user pool
- **calculate_resource_usage**: Check if custom attributes and Lambda triggers stay within Cognito limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cognito User Pool Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 1.5 million users and 150 app clients. How many user pools do I need?"

**🤖 AI Agent:**
> You will need 2 user pools to stay within the recommended 1 million users per pool limit.

---

**👤 You:**
> "What is the total size of my JWT tokens if I use standard settings?"

**🤖 AI Agent:**
> The total token size is approximately 3.25 KB (2 KB for the ID token, 1 KB for the access token, and 256 bytes for the refresh token).

---

**👤 You:**
> "I want to use 60 custom attributes. Is this allowed?"

**🤖 AI Agent:**
> No, the limit for custom attributes is 50. You will need to reduce your custom attribute count to stay within the architectural limits.


## ❓ FAQ

**Q: How many users can I fit in one Cognito pool?**
While there is no hard limit, it is recommended to keep a single pool under 1 million users for optimal performance. You can use `calculate_pool_capacity` to see if you need to split your users into multiple pools.

**Q: Can I check my custom attribute limits?**
Yes, use `calculate_resource_usage` to verify if your custom attribute count is within the 50-attribute limit and if your standard attributes are within the 20-attribute limit.

**Q: How do I estimate SMS costs and limits?**
You can use `estimate_sms_throughput` to calculate the theoretical maximum daily SMS messages for your user base and check if you will exceed the account-wide limit of 10,000 messages per day.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/cognito-user-pool-calculator](https://vinkius.com/ai-agent-connect/cognito-user-pool-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cognito User Pool Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cognito-user-pool-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cognito User Pool Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cognito-user-pool-calculator": {
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
