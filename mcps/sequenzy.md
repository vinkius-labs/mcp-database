# Sequenzy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sequenzy)
[![Built with MCP](https://img.shields.io/badge/Protocol-MCP-success?style=for-the-badge)](https://github.com/Sequenzy/mcp)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Operate permissioned lifecycle, campaign, and transactional email workflows in Sequenzy from AI agents.

## Description

Connect your **Sequenzy** account to MCP-compatible agents to manage customer email operations through natural language. Sequenzy is designed for owned-audience SaaS and ecommerce messaging: subscribers, lists, segments, templates, campaigns, sequences, transactional email, inbox replies, webhooks, and delivery statistics.

### What you can do

- **Subscriber and list operations** — create, update, tag, segment, and inspect opted-in contacts.
- **Lifecycle campaigns** — draft, schedule, and monitor product, onboarding, retention, and ecommerce email campaigns.
- **Sequences and automations** — build and inspect multi-step lifecycle journeys for existing users and customers.
- **Transactional email** — send and audit operational emails with template and delivery visibility.
- **Performance and reply review** — inspect campaign stats, delivery state, lead/customer history, and inbound replies before taking action.

### How it works

1. Install the Sequenzy MCP server from the public package or connect to the hosted remote endpoint.
2. Authenticate with a Sequenzy API key or account-linked remote session.
3. Use Claude, Cursor, Codex, Hermes, or another MCP-compatible client to operate email workflows.
4. Keep usage permissioned: Sequenzy is for lifecycle, campaign, and transactional email to owned audiences, not unsolicited cold outreach.

### Who is this for?

- **SaaS founders and growth teams** — run onboarding, activation, retention, and product-update campaigns from agents.
- **Ecommerce operators** — manage customer segments, promotional campaigns, and post-purchase messaging.
- **Developers** — connect application events and transactional email workflows to agent-operated tooling.
- **Marketing operations teams** — audit templates, stats, segments, and replies without hand-clicking through dashboards.

## Available Tools

Sequenzy exposes MCP tools for common email marketing and operational workflows, including subscribers, lists, tags, segments, campaigns, templates, sequences, transactional sends, inbox replies, webhooks, analytics, and account metadata. See the canonical repository for the current tool list and install options.

## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sequenzy** MCP server using an AI Agent (Claude, Cursor, Codex, Hermes, etc.).

**👤 You:**
> "Create a segment of activated trial users who have not started onboarding step 3, draft a lifecycle email for them, and show me the audience count before scheduling."

**🤖 AI Agent:**
> I found the matching trial users, drafted a permissioned lifecycle email, and paused before scheduling so you can approve the audience and copy.

---

**👤 You:**
> "Check whether yesterday's onboarding campaign had bounce or reply issues, then summarize what needs attention."

**🤖 AI Agent:**
> I reviewed delivery stats and recent replies, flagged hard bounces and customer questions, and grouped the follow-up actions by priority.

---

**👤 You:**
> "Send a transactional receipt email using the receipt template for this customer and verify delivery status afterwards."

**🤖 AI Agent:**
> I sent the transactional email with the requested template and checked the delivery event so you can confirm it was accepted.

## Installation & Usage

### Claude Desktop / Cursor / local MCP clients

Use the public npm package:

```json
{
  "mcpServers": {
    "sequenzy": {
      "command": "npx",
      "args": ["-y", "@sequenzy/mcp"],
      "env": {
        "SEQUENZY_API_KEY": "your_api_key_here"
      }
    }
  }
}
```

### Remote MCP endpoint

Sequenzy also publishes a hosted Streamable HTTP endpoint:

```text
https://api.sequenzy.com/v1/mcp
```

Use OAuth/account-linking or the authentication method documented by your MCP client when connecting to the hosted endpoint.

## Links

- Repository: [https://github.com/Sequenzy/mcp](https://github.com/Sequenzy/mcp)
- Package: [https://www.npmjs.com/package/@sequenzy/mcp](https://www.npmjs.com/package/@sequenzy/mcp)
- Website: [https://sequenzy.com](https://sequenzy.com)

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by Sequenzy. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This entry describes the public Sequenzy MCP server for agent-operated email marketing workflows.*
