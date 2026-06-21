# All Digital Rewards MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/all-digital-rewards)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Incentive and reward orchestration — manage participants, points, and catalogs via AI.

## Description
Connect your **All Digital Rewards (RewardSTACK™)** account to your AI agent to unlock professional incentive program management. From registering new participants and issuing behavior-based points to auditing reward catalogs and monitoring fulfillment orders, your agent handles your engagement strategy through natural conversation.

### What you can do

- **Participant Orchestration** — Register new participants and retrieve detailed profiles, including point balances and activity history
- **Reward Catalog Oversight** — List available digital and physical rewards, including gift cards and merchandise from global brands
- **Incentive Management** — Issue points programmatically to reward specific user behaviors or milestones
- **Order Monitoring** — List and audit reward redemption orders and track their fulfillment status in real-time
- **Program Intelligence** — Quickly identify top participants or audit reward availability directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your RewardSTACK Email and Password
3. Start managing your incentive programs and monitoring rewards through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **HR & People Ops** — automate employee recognition programs and reward distribution
- **Marketing Managers** — manage customer loyalty incentives and track gift card redemptions
- **Sales Leaders** — issue performance bonuses and monitor sales contest rewards effortlessly
- **Customer Success** — provide instant rewards for customer referrals or milestones using simple commands


## Available Tools (10)
- **list_programs**: List incentive programs
- **get_program_details**: Get program metadata
- **list_participants**: List reward participants
- **get_participant_details**: Get participant profile
- **create_participant**: Enroll new user
- **issue_points**: Reward behavior with points
- **list_reward_products**: List available rewards
- **get_product_details**: Get reward metadata
- **list_orders**: List redemption orders
- **get_order_details**: Get order fulfillment status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **All Digital Rewards** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active incentive programs in my account."

**🤖 AI Agent:**
> I've retrieved your programs. You have 3 active incentive structures: 'Employee Wellness 2026', 'Customer Loyalty Platinum', and 'Q1 Sales Contest'. Would you like to see the participant count for any of these?

---

**👤 You:**
> "Issue 500 points to participant ID 'part_12345' for 'Excellence Award'."

**🤖 AI Agent:**
> I've successfully issued 500 points to participant part_12345. Their new balance is 1,250 points. The transaction has been logged under the 'Excellence Award' reason. Would you like to see their full transaction history?

---

**👤 You:**
> "List the top 5 most popular rewards in my catalog."

**🤖 AI Agent:**
> I've analyzed your reward catalog. The top 5 most redeemed items are: 1. $50 Amazon Gift Card, 2. $25 Starbucks Card, 3. Noise-cancelling Headphones, 4. Wireless Mouse, and 5. $100 Visa Prepaid Card. Would you like to check the current stock for the physical items?


## ❓ FAQ

**Q: How do I find my RewardSTACK API credentials?**
Use your standard RewardSTACK administrative email and password. Your AI agent will use these to obtain a temporary JWT (JSON Web Token) for all API requests.

**Q: Can I issue points to multiple participants at once?**
The `issue_points` tool currently processes points for a specific participant ID. For bulk processing, you can ask your agent to loop through a list of IDs or use the RewardSTACK batch file upload feature.

**Q: What types of rewards are available in the catalog?**
The Reward Catalog API provides access to thousands of digital gift cards (Visa, Amazon, etc.), physical merchandise from major retailers, and unique experiential rewards.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/all-digital-rewards](https://vinkius.com/mcp/all-digital-rewards)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **All Digital Rewards** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `all-digital-rewards` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **All Digital Rewards** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "all-digital-rewards": {
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
