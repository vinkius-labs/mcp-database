# Accessible Ticketing Decision Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-ticketing-decision-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Evaluates ticket availability and purchase feasibility by prioritizing mandatory accessibility needs and budget constraints.

## Description
This MCP server provides a decision engine to help users navigate complex ticketing requirements. It prioritizes non-negotiable accessibility needs--such as wheelchair access or sensory accommodations--over personal preferences. By using tools like `analyze_ticket_feasibility` and `determine_fallback_option`, the engine ensures that selected tickets meet both physical requirements and strict budget ceilings. It also generates logistical checklists and validates compliance with venue-specific refund and participation policies.


## Available Tools (4)
- **determine_fallback_option**: Provide a secondary choice if the primary ticket is unavailable
- **analyze_ticket_feasibility**: Determine if a ticket type meets accessibility and budget constraints
- **generate_purchase_checklist**: Produce a list of logistical actions for the purchase
- **validate_compliance_terms**: Extract and format legal terms and venue features


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Ticketing Decision Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if a $150 ticket is feasible for someone needing wheelchair access with a $200 budget and a required companion."

**🤖 AI Agent:**
> The ticket is feasible. The total cost including the companion is $300, which exceeds your budget. However, if the companion is free, the total is $150, which is within your $200 limit.

---

**👤 You:**
> "Generate a purchase checklist for a concert with a deadline of tomorrow and a companion policy requiring ID."

**🤖 AI Agent:**
> Please complete your purchase by tomorrow. Ensure you have valid identification ready for both yourself and your companion as per the venue policy.

---

**👤 You:**
> "What are the refund terms and relevant venue features for this event?"

**🤖 AI Agent:**
> Refunds are available up to 24 hours before the event. The venue features include ramps and hearing loops which match your requirements.


## ❓ FAQ

**Q: How does the engine handle accessibility needs?**
The engine uses `analyze_ticket_feasibility` to ensure that mandatory accessibility requirements are satisfied before considering any other preferences or budget factors.

**Q: What happens if my first choice of ticket is unavailable?**
You can use the `determine_fallback_option` tool to find an alternative ticket that still respects your mandatory accessibility needs and budget ceiling.

**Q: Does the tool account for companion tickets?**
Yes, the feasibility analysis includes the cost of companion tickets if they are required by the venue's companion policy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-ticketing-decision-plan](https://vinkius.com/en/ai-agent-connect/accessible-ticketing-decision-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Ticketing Decision Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-ticketing-decision-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Ticketing Decision Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-ticketing-decision-plan": {
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
