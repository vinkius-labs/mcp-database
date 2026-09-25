# Community Space Booking Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/community-space-booking-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Evaluate venue suitability, timelines, and setup needs for community events.

## Description
This MCP server provides decision-support tools for event organizers. It evaluates venue suitability by matching attendee counts, budget constraints, and equipment needs. Use `analyze_venue_suitability` to rank venues, `generate_booking_timeline` to check lead times, `generate_contract_questions` to identify logistical friction points, and `create_setup_checklist` to prepare the physical space.


## Available Tools (4)
- **create_setup_checklist**: Produce a task list for event organizers to prepare the venue
- **generate_booking_timeline**: Determine if the requested dates are feasible based on venue-specific lead times
- **analyze_venue_suitability**: Rank available venues by comparing event requirements against venue properties
- **generate_contract_questions**: Identify potential legal or logistical friction points that require manual clarification


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Community Space Booking Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to host a meeting for 50 people with a budget of $500. We need a projector and wheelchair access. Which venues work?"

**🤖 AI Agent:**
> The Community Center is the best match with a total cost of $450, providing both the projector and wheelchair access.

---

**👤 You:**
> "Is it too late to book a venue for an event on December 20th if the venue requires 30 days notice?"

**🤖 AI Agent:**
> No, since today is November 1st, you have 50 days of notice, which satisfies the 30-day requirement.

---

**👤 You:**
> "What should I prepare for an event that requires a sound system and ramp access?"

**🤖 AI Agent:**
> You should ensure the sound system is tested for connectivity and verify that the ramp is clear of obstructions for accessibility.


## ❓ FAQ

**Q: How does the venue ranking work?**
The `analyze_venue_suitability` tool ranks venues based on a match score that considers capacity, required features, accessibility, and total cost including equipment.

**Q: Can I check if my event date is too late to book?**
Yes, use `generate_booking_timeline` to compare your event date against the specific lead-time requirements of each venue.

**Q: What kind of checklist will I receive?**
The `create_setup_checklist` tool generates actionable tasks categorized by Equipment, Accessibility, or General needs based on your requirements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/community-space-booking-plan](https://vinkius.com/en/ai-agent-connect/community-space-booking-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Community Space Booking Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `community-space-booking-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Community Space Booking Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "community-space-booking-plan": {
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
