# Accessible Home Visitor Protocol MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-home-visitor-protocol)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication](../categories/communication.md)

Structured, privacy-preserving communication flows for managing visitor access and resident needs.

## Description
This MCP server acts as a bridge between residents with specific accessibility requirements and their visitors. It transforms individual needs, household boundaries, and building entry rules into structured communication flows. By using tools like `generate_pre_visit_briefing` and `orchestrate_handoff`, the protocol ensures visitors are prepared before arrival and transitions smoothly into the home while strictly respecting privacy and resident consent through `initiate_privacy_feedback`.


## Available Tools (4)
- **get_entry_protocol**: Tells the visitor exactly how to navigate the building's exterior and entry points
- **generate_pre_visit_briefing**: Provides the visitor with everything they need to know before they arrive
- **initiate_privacy_feedback**: Facilitates a post-visit review that allows the resident to confirm protocol adherence
- **orchestrate_handoff**: Manages the transition from the visitor's arrival to the actual interaction with the resident


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Home Visitor Protocol** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Prepare a briefing for a medical professional arriving at 2 PM, noting that the resident needs low lighting and there is a quiet period scheduled."

**🤖 AI Agent:**
> Briefing prepared: The visitor will receive instructions regarding the low lighting requirement and a specific warning about the scheduled quiet period to ensure compliance.

---

**👤 You:**
> "The visitor has arrived at the gate. How should they enter and contact the resident?"

**🤖 AI Agent:**
> The visitor should use the gate code 1234 and then send a text message to the resident as requested.

---

**👤 You:**
> "The maintenance worker is inside. Remind them of the boundaries and the resident's needs."

**🤖 AI Agent:**
> The worker is instructed to stay in the kitchen and avoid the second bedroom, while ensuring they provide verbal cues as requested by the resident.


## ❓ FAQ

**Q: How does this protocol protect resident privacy?**
The protocol uses a tiered information system and the `initiate_privacy_feedback` tool to ensure only necessary context is shared with visitors, masking sensitive data.

**Q: Can I use this for delivery personnel?**
Yes. By using `get_entry_protocol`, you can provide couriers with specific building rules and contact methods without revealing sensitive household details.

**Q: What happens if a visitor ignores household boundaries?**
Residents can use the `initiate_privacy_feedback` tool after a visit to report if the protocol was followed, helping to refine future instructions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-home-visitor-protocol](https://vinkius.com/en/ai-agent-connect/accessible-home-visitor-protocol)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Home Visitor Protocol** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-home-visitor-protocol` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Home Visitor Protocol** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-home-visitor-protocol": {
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
