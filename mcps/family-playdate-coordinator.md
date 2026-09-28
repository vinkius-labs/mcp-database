# Family Playdate Coordinator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-playdate-coordinator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [social](../categories/social.md)

Manage multi-family playdate logistics, safety, and handoff protocols.

## Description
This MCP server provides a specialized coordination engine for managing the complexities of multi-household social gatherings. It enforces critical safety and logistics constraints including Consent-Before-Confirmation, Capacity Management, and Host Responsibility. Use `generate_invitations` to draft formal invites, `calculate_attendance_roster` to verify capacity limits, `create_preparation_checklist` to manage dietary needs and household rules, and `plan_transport_handoff` to ensure children are only released to authorized contacts.


## Available Tools (4)
- **generate_invitations**: Creates formal invitation drafts based on the proposed playdate details
- **plan_transport_handoff**: Creates a schedule for the arrival and departure of children, ensuring authorized transport
- **calculate_attendance_roster**: Generates the final list of confirmed attendees and checks capacity limits
- **create_preparation_checklist**: Produces a logistical checklist for the host based on dietary needs and household rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Playdate Coordinator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate invitations for the Smith and Jones families for a playdate on June 12th at 123 Maple St."

**🤖 AI Agent:**
> I have generated the invitation drafts for the Smith and Jones families for June 12th at 123 Maple St. They are currently in pending status.

---

**👤 You:**
> "Check if we have enough space for 10 people at our house for the playdate."

**🤖 AI Agent:**
> The current attendance roster shows 8 confirmed attendees, which is within your capacity of 10.

---

**👤 You:**
> "Create a checklist for the host including the rule 'No shoes indoors' and the allergy 'Peanut allergy for Leo'."

**🤖 AI Agent:**
> The preparation checklist includes the rule 'No shoes indoors' and highlights the peanut allergy for Leo as a dietary requirement.


## ❓ FAQ

**Q: How does the server handle capacity limits?**
The `calculate_attendance_roster` tool checks the total number of confirmed adults and children against the provided `locationCapacity` and throws an error if the limit is exceeded.

**Q: Can I ensure only authorized people pick up my children?**
Yes. The `plan_transport_handoff` tool validates every transport contact against the list of authorized contacts provided for each child.

**Q: How are dietary restrictions managed?**
The `create_preparation_checklist` tool aggregates all unique dietary requirements from confirmed families to create a specific preparation list for the host.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-playdate-coordinator](https://vinkius.com/en/ai-agent-connect/family-playdate-coordinator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Playdate Coordinator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-playdate-coordinator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Playdate Coordinator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-playdate-coordinator": {
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
