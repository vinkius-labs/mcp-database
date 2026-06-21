# FastSpring MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fastspring)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage digital commerce via FastSpring — track orders and subscriptions, handle accounts, and manage product catalogs directly from any AI agent.

## Description
Connect your **FastSpring** account to any AI agent and take full control of your digital commerce, global payments, and subscription management through natural conversation.

### What you can do

- **Order & Transaction Auditing** — Retrieve explicit cloud logs tracing order limits and resolve if customers successfully passed fraud filtering natively
- **Subscription Orchestration** — Inspect deep internal arrays for renewals, check currency applications, and handle ad-hoc charges or plan updates flawlessly
- **Account Management** — Identify and update bounded CRM records, managing customer emails and profile data across the headless FastSpring platform
- **Churn Control** — Irreversibly vaporize explicit validations to cancel managed subscriptions securely while extracting rich churn reason metadata
- **Catalog & Product Navigation** — Retrieve exact structural matching for configured packages and verify which digital products are active in your store
- **Authentication Linkage** — Dispatch automated validation checks generating ephemeral 24h JWT links for customer portal access securely
- **Revenue Recovery** — Execute bulk iterations to manually trigger subscription renewals and manage MoR revenue arrays synchronously

### How it works

1. Subscribe to this server
2. Enter your FastSpring API Username and Password (found in Dashboard > Integrations > Store Settings > API Credentials)
3. Start managing your digital commerce from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SaaS Founders & Managers** — monitor subscription health and manage customer accounts without manual dashboard navigation
- **Customer Success Teams** — quickly look up order details and generate authentication links to resolve customer inquiries
- **Operations Teams** — audit product catalogs and verify global payment statuses using natural language
- **Developers** — test and debug commerce integrations and verify subscription proration logic through natural conversation


## Available Tools (10)
- **cancel_subscription**: Irreversibly vaporize explicit validations extracting rich Churn flags
- **charge_managed_subscription**: Enumerate explicitly attached structured rules exporting active Billing
- **get_account_details**: Perform structural extraction of properties driving active Account logic
- **generate_auth_link**: Dispatch an automated validation check routing explicit Login tokens
- **get_order_details**: Retrieve explicit Cloud logging tracing explicit Ordering limits
- **get_subscription_details**: Inspect deep internal arrays mitigating specific Plan Math
- **list_accounts**: Identify bounded CRM records inside the Headless FastSpring Platform
- **list_catalog_products**: Retrieve the exact structural matching verifying Product mapping
- **update_account_info**: Provision a highly-available JSON Payload generating hard Customer updates
- **update_subscription_plan**: Identify precise active arrays spanning native Plan tracking


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FastSpring** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the status of FastSpring order 'ORD-12345'?"

**🤖 AI Agent:**
> Retrieving order details... Order ORD-12345 is currently 'Completed'. The customer successfully passed fraud filtering and the license keys have been delivered. Would you like the buyer's email address?

---

**👤 You:**
> "Generate a 24h auth link for account 'acc_abc123'"

**🤖 AI Agent:**
> Auth link generated! Here is the ephemeral login URL for account acc_abc123: https://yourstore.onfastspring.com/authenticate/jwt... This link will expire in 24 hours.

---

**👤 You:**
> "Cancel subscription 'sub_xyz789' and tell me why"

**🤖 AI Agent:**
> Subscription cancelled! sub_xyz789 has been terminated. The recorded churn metadata indicates the reason was 'Price too high'. The customer will no longer be charged for this plan.


## ❓ FAQ

**Q: Can my agent check if an order passed fraud filtering in FastSpring?**
Yes. Use the 'get_order_details' tool. The agent retrieves explicit cloud logs resolving if customers successfully passed fraud checks, providing you with the exact status of any transaction UUID.

**Q: How do I generate a customer login link via chat?**
Use the 'generate_auth_link' tool. Provide the account ID. Your agent will command the FastSpring API to generate an ephemeral 24h JWT link that grants the customer secure access to their portal without a password.

**Q: Can I manually trigger a renewal charge for a subscription through the agent?**
Absolutely. Use the 'charge_managed_subscription' tool. Providing the sub ID allows the agent to execute a manual renewal charge via the MoR infrastructure, handling the ad-hoc billing event synchronously.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fastspring](https://vinkius.com/mcp/fastspring)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FastSpring** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fastspring` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FastSpring** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fastspring": {
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
