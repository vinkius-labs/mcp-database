# Referly MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/referly)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate affiliate programs via Referly — manage partners, track conversions, and monitor workflows directly.

## Description
Connect your **Referly** (referly.so) account to any AI agent and take full control of your referral marketing and affiliate orchestration through natural conversation. Referly provides a powerful platform for managing partners and conversion tracking, and this integration allows you to retrieve affiliate metadata, trigger custom referral workflows, and monitor program performance directly from your chat interface.

### What you can do

- **Affiliate & Partner Orchestration** — List all managed affiliates and retrieve detailed performance metadata, including creating new partner profiles programmatically.
- **Referral & Conversion Intelligence** — Track real-time conversion events and attribute sign-ups or sales to specific referral codes directly from the AI interface.
- **Workflow & Automation Control** — Trigger custom referral workflows and monitor their execution statuses via natural language to keep your growth loops synchronized.
- **Coupon & Promo Oversight** — Validate discount coupons and list active promo codes to ensure your marketing campaigns are always optimized.
- **Operational Monitoring** — Access analytics summaries and manage tenant metadata using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your Referly Tenant ID and API Key from your dashboard at referly.so
3. Start managing your growth programs from Claude, Cursor, or any MCP-compatible client

No more manual CSV exports or attribute hunting. Your AI acts as a dedicated growth manager or affiliate coordinator.

### Who is this for?

- **Growth Marketers** — quickly retrieve referral stats and monitor partner performance without switching apps.
- **Partnership Managers** — automate the onboarding of new affiliates and track their impact via natural conversation.
- **Operations Teams** — streamline the retrieval of conversion metadata and monitor organizational growth health directly within the chat.


## Available Tools (12)
- **create_affiliate**: Requires name and email.

Create a new affiliate
- **get_affiliate_details**: Get details for a specific affiliate
- **get_referral_analytics**: Get referral performance summary
- **get_current_user**: Get authenticated user profile
- **get_workflow_status**: Check workflow execution status
- **list_affiliates**: List all affiliates/partners
- **list_coupons**: List all discount coupons
- **list_referrals**: List all referral events
- **list_referral_workflows**: List automation workflows
- **trigger_workflow**: Manually trigger a workflow
- **track_referral_event**: Track a new referral conversion
- **validate_coupon**: Validate a discount coupon


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Referly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active affiliates in my Referly account."

**🤖 AI Agent:**
> I've retrieved your affiliates. You have 3 active partners: 'Main Agency', 'Tech Reviewer' (ID: 991), and 'Vinkius Affiliate'. Which one would you like to see conversions for?

---

**👤 You:**
> "Show me the performance of all active referral programs with conversion rates this month."

**🤖 AI Agent:**
> 4 active referral programs. "Customer Ambassador" leads with 234 referrals and 18% conversion (42 new paying customers). Revenue attributed: $12,600. "Partner Affiliate" generated 156 referrals with 24% conversion and $8,900 in commissions paid. "Employee Referral" submitted 12 candidates, 4 hired (33% success rate). "Influencer Program" produced 890 clicks and 34 signups. Total referral-driven revenue: $28,400. Top referrer: Sarah Chen with 23 successful conversions earning $1,380.

---

**👤 You:**
> "Create a new referral campaign offering $50 credit for each successful customer referral."

**🤖 AI Agent:**
> Referral campaign created: "Refer & Earn $50". Reward: $50 account credit per successful referral. Qualification: referred user must complete signup and make first purchase. Double-sided: referrer gets $50, referred friend gets $25. Tracking link generated for each participant. Email notification template configured. Landing page created with shareable social media buttons. Campaign status: Active. Budget cap: $5,000 (100 referrals).


## ❓ FAQ

**Q: Can my AI automatically find if a specific discount code is valid in Referly?**
Yes! Use the `validate_coupon` tool. Provide the promo code, and your agent will return its eligibility status and technical metadata instantly.

**Q: How do I find my Referly Tenant ID and API Key?**
Log in to your Referly dashboard at referly.so, navigate to **Settings** > **API Keys**, and you will find your unique Tenant ID and secret API key there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/referly](https://vinkius.com/mcp/referly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Referly** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `referly` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Referly** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "referly": {
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
