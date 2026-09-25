# Care Social Visit Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/care-social-visit-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Coordinates balanced social schedules, invitations, and transport based on energy limits and accessibility needs.

## Description
This MCP server acts as an intelligent coordination engine for individuals managing energy levels and social needs. It uses `plan_social_calendar` to create balanced schedules that respect energy constraints and recovery spacing. It can `generate_invitations` with personalized messaging, `assign_transport` by matching accessibility requirements to available vehicles, and provide a `get_cancellation_protocol` to handle unexpected energy depletion gracefully.


## Available Tools (4)
- **assign_transport**: Matches transport requirements to the specific needs of the user for each planned visit
- **plan_social_calendar**: Generates a structured schedule of visits based on available dates, guest availability, and energy constraints
- **generate_invitations**: Creates personalized, respectful invitation messages for the approved guests
- **get_cancellation_protocol**: Provides a standardized set of instructions and communication templates for canceling a visit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Care Social Visit Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a social calendar for next week with an energy limit of 50 units using these guests: Alice (10 units), Bob (15 units), and Charlie (20 units)."

**🤖 AI Agent:**
> I have created a balanced schedule for next week: Monday with Alice (10 units), Wednesday with Bob (15 units), and Friday with Charlie (20 units). Your remaining energy is 5 units.

---

**👤 You:**
> "Generate an invitation for Bob for our scheduled meal on Wednesday."

**🤖 AI Agent:**
> Hi Bob, I would love for you to join me for a meal this Wednesday. Looking forward to it!

---

**👤 You:**
> "I need to cancel my visit with Charlie because my energy is too low. My current energy is 5."

**🤖 AI Agent:**
> I have prepared the cancellation protocol. You can send this message to Charlie: 'Hi Charlie, I'm feeling a bit low on energy today and need to reschedule our visit. I hope you understand!'


## ❓ FAQ

**Q: How does the tool manage my energy levels?**
The `plan_social_calendar` tool calculates the energy cost of each activity and ensures the total does not exceed your defined limit, while also maintaining necessary recovery time between visits.

**Q: Can I use this to organize transport for my guests?**
Yes, the `assign_transport` tool matches your specific accessibility needs with available vehicles to ensure safe and comfortable travel for every visit.

**Q: What happens if I run out of energy unexpectedly?**
You can use `get_cancellation_protocol` to receive standardized instructions and polite, guilt-free messages to notify hosts and guests about cancellations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/care-social-visit-plan](https://vinkius.com/en/ai-agent-connect/care-social-visit-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Care Social Visit Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `care-social-visit-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Care Social Visit Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "care-social-visit-plan": {
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
