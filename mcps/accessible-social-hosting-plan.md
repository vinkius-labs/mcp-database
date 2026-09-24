# Accessible Social Hosting Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-social-hosting-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Organize inclusive gatherings by matching guest accessibility needs with home features and household boundaries.

## Description
This MCP server provides a coordination system for hosts to organize social gatherings that respect physical accessibility needs, privacy boundaries, and household logistics. It allows AI agents to generate a complete hosting blueprint, including spatial layouts via `get_hosting_arrangement`, guest communication drafts via `get_guest_communication`, task assignments via `get_responsibilities_plan`, and structured departure protocols via `get_closeout_plan`. It ensures that guest requirements are safely matched against home features while strictly honoring host-defined boundaries.


## Available Tools (4)
- **get_closeout_plan**: Defines how the event concludes to respect the host's time and household limits
- **get_hosting_arrangement**: Generates the spatial and logistical layout for the gathering
- **get_responsibilities_plan**: Assigns specific tasks to the host and support people for the start of the event
- **get_guest_communication**: Drafts the information to be sent to guests to prepare them for the event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Social Hosting Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 5 guests. My home has wide doorways and a ground floor. One guest needs wheelchair access. My boundaries are: no access to the upstairs office."

**🤖 AI Agent:**
> The hosting arrangement is set for the ground floor. The wide doorways accommodate the wheelchair access requirement. The upstairs office remains a restricted zone per your boundaries.

---

**👤 You:**
> "Draft a message for my guests. They need quiet zones. The event is from 6 PM to 10 PM. Guests must stay in the living room and dining area."

**🤖 AI Agent:**
> Hello! We look forward to seeing you from 6 PM to 10 PM. Please note that the gathering will be held in the living room and dining area. We have identified quiet zones to accommodate your needs.

---

**👤 You:**
> "Help me plan the end of my event. It lasts from 2 PM to 5 PM. I need to ensure guests respect the 'no entry to bedroom' rule when leaving."

**🤖 AI Agent:**
> The event will conclude at 5 PM. The departure process will guide guests through the main exit, ensuring the bedroom remains a restricted area as requested.


## ❓ FAQ

**Q: How does the server handle accessibility mismatches?**
The `get_hosting_arrangement` tool compares guest requirements against home features and will explicitly flag any mismatches in the accessibility notes.

**Q: Can I define specific areas that are off-limits?**
Yes, you can define hosting boundaries. Tools like `get_guest_communication` and `get_closeout_plan` use these boundaries to ensure guests are informed and household limits are respected.

**Q: How are tasks assigned to helpers?**
The `get_responsibilities_plan` tool distributes arrival and seating tasks among the support people you provide.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-social-hosting-plan](https://vinkius.com/en/ai-agent-connect/accessible-social-hosting-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Social Hosting Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-social-hosting-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Social Hosting Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-social-hosting-plan": {
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
