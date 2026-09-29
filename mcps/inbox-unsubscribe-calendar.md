# Inbox Unsubscribe Calendar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/inbox-unsubscribe-calendar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate optimized review schedules to prune email subscriptions and reduce inbox noise.

## Description
This MCP server helps users manage inbox clutter by creating structured review sessions. It identifies high-impact senders that contribute most to inbox noise and organizes them into manageable batches based on your review capacity. You can use `get_sender_priority_batches` to find the best groups to review, `calculate_expected_reduction` to see how many emails you will save, `get_sender_impact_analysis` to understand why a sender is a priority, and `generate_review_schedule` to build a complete roadmap for cleaning your inbox.


## Available Tools (4)
- **calculate_expected_reduction**: Estimates how many emails will be removed from the inbox if the user unsubscribes from specific senders
- **generate_review_schedule**: Generates a full roadmap of review sessions over time
- **get_sender_impact_analysis**: Retrieves a detailed breakdown of why a specific sender is or is not a priority for review
- **get_sender_priority_batches**: Provides a prioritized list of sender groups to review to maximize inbox cleaning efficiency


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Inbox Unsubscribe Calendar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a list of the most important senders to review, with a capacity of 5 senders per session."

**🤖 AI Agent:**
> Here are your prioritized batches: Batch 1 includes newsletter-daily@example.com and promo-deals@example.com. Unsubscribing from these will reduce your inbox volume by 15 emails per week.

---

**👤 You:**
> "How many emails will I save if I unsubscribe from news@example.com and alerts@example.com?"

**🤖 AI Agent:**
> You will save approximately 42 emails per week by unsubscribing from those two senders.

---

**👤 You:**
> "Create a review schedule starting tomorrow where I can review 3 senders per day."

**🤖 AI Agent:**
> Your review schedule is ready. On 2024-05-20, you will review 3 senders. On 2024-05-21, you will review another 3 senders.


## ❓ FAQ

**Q: How does the tool decide which senders to review first?**
The tool uses `get_sender_priority_batches` to rank senders by their impact score, which is a combination of how frequently they send emails and how recently they were received.

**Q: Can I control how many emails I review at once?**
Yes, you can specify your `reviewCapacity` to ensure you only audit a number of senders that fits your availability.

**Q: How accurate is the predicted email reduction?**
The `calculate_expected_reduction` tool provides an estimate based on sender frequency, with higher confidence for more frequent senders.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/inbox-unsubscribe-calendar](https://vinkius.com/en/ai-agent-connect/inbox-unsubscribe-calendar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Inbox Unsubscribe Calendar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `inbox-unsubscribe-calendar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Inbox Unsubscribe Calendar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "inbox-unsubscribe-calendar": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
