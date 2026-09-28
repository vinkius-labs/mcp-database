# Local Group Reservation Coordinator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/local-group-reservation-coordinator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Coordinates group reservations by aligning participant commitments with venue policies.

## Description
This MCP server provides a structured coordination engine for managing group bookings. It uses tools like `generate_reservation_request` to create formal venue requests, `create_attendee_confirmation` to secure participant commitment, and `map_responsibilities` to define roles. It also handles logistics via `draft_change_notifications` and `define_contingency_plan` to manage capacity issues or policy changes.


## Available Tools (5)
- **define_contingency_plan**: Develops a step-by-step procedure to follow if the reservation cannot be completed
- **draft_change_notifications**: Generates notification templates for when the reservation details change
- **generate_reservation_request**: Creates a formal request to be sent to the venue based on the experience and participant data
- **map_responsibilities**: Produces a clear list of who is responsible for what, distinguishing between the organizer and the participants
- **create_attendee_confirmation**: Generates a sequence of messages to confirm individual participation and acknowledge their commitment to the venue terms


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Local Group Reservation Coordinator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a reservation request for a group of 8 people for the 'Sunset Dinner' experience. The venue limit is 10 and the policy is 'No late arrivals'."

**🤖 AI Agent:**
> Reservation Request: We would like to request a reservation for 8 guests for the Sunset Dinner. We acknowledge the policy of no late arrivals.

---

**👤 You:**
> "Create confirmation messages for Alice, Bob, and Charlie. The policy is that everyone must pay individually."

**🤖 AI Agent:**
> Alice, Bob, and Charlie: Your participation is confirmed. You have agreed to the policy requiring individual payments.

---

**👤 You:**
> "What should I do if the group size changes and we have too many people?"

**🤖 AI Agent:**
> You should use `define_contingency_plan` with the reason 'overcapacity' to receive a step-by-step procedure for reducing the list or finding a new venue.


## ❓ FAQ

**Q: How does the tool ensure venue compliance?**
The `generate_reservation_request` tool validates the participant count against the specific `groupSizeLimit` provided by the venue to ensure all rules are met.

**Q: What happens if the group exceeds the venue capacity?**
You can use `define_contingency_plan` to trigger a procedure that prioritizes finding a secondary venue or reducing the participant list.

**Q: Can I manage participant responsibilities?**
Yes, the `map_responsibilities` tool creates a clear list distinguishing between the Contact Owner's tasks and the participants' obligations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/local-group-reservation-coordinator](https://vinkius.com/en/ai-agent-connect/local-group-reservation-coordinator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Local Group Reservation Coordinator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `local-group-reservation-coordinator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Local Group Reservation Coordinator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "local-group-reservation-coordinator": {
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
