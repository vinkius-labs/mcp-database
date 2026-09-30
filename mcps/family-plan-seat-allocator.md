# Family Plan Seat Allocator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-plan-seat-allocator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Intelligently assigns household members to family plan seats based on priority and storage.

## Description
This MCP server provides a specialized engine for managing family plan subscriptions. It automates the process of matching household members to available seats by evaluating their priority levels, current service usage, and digital storage requirements. Use `allocate_family_seats` to perform core seat matching, `validate_member_eligibility` to check member constraints, `calculate_storage_utilization` to monitor quota usage, and `identify_subscription_conflicts` to detect overlapping individual subscriptions.


## Available Tools (4)
- **allocate_family_seats**: Performs the core logic of matching household members to available family plan seats
- **calculate_storage_utilization**: Determines how much of the plan's storage quota is consumed by a specific set of assignments
- **identify_subscription_conflicts**: Scans the household to find members who currently pay for services that would overlap with the family plan
- **validate_member_eligibility**: Checks if a specific member is technically eligible to be added to a plan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Plan Seat Allocator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Allocate seats for these members: 3 members, capacity 2, total storage 100GB. Member A (Priority 1, 60GB), Member B (Priority 2, 30GB), Member C (Priority 3, 20GB)."

**🤖 AI Agent:**
> Member A is assigned a seat. Member B is assigned a seat. Member C remains unassigned due to storage limits. Unused seats: 0. Duplicate subscriptions: 0.

---

**👤 You:**
> "Check if a member with ID 'user_123' is eligible for a plan with age limit 18."

**🤖 AI Agent:**
> The member is eligible for the plan.

---

**👤 You:**
> "Calculate the storage utilization for 2 assigned members using 40GB and 50GB of a 100GB quota."

**🤖 AI Agent:**
> Used storage is 90GB, remaining storage is 10GB, and utilization is 90%.


## ❓ FAQ

**Q: How does the seat allocation priority work?**
The engine processes members in descending order of their priority tier. Higher priority members are assigned seats first until either the `planCapacity` is reached or the `totalStorageQuota` is exhausted.

**Q: What happens if a member's storage needs are too high?**
If a member's storage requirement exceeds the remaining available quota, they will remain unassigned even if there are still available seats in the plan.

**Q: How can I find members with duplicate subscriptions?**
You can use the `identify_subscription_conflicts` tool to scan the household list and find members who already pay for services covered by the family plan.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-plan-seat-allocator](https://vinkius.com/en/ai-agent-connect/family-plan-seat-allocator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Plan Seat Allocator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-plan-seat-allocator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Plan Seat Allocator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-plan-seat-allocator": {
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
