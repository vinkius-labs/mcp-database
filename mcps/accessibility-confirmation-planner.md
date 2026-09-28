# Accessibility Confirmation Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessibility-confirmation-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Plan accessibility logistics and contact sequences for local experiences.

## Description
This MCP server provides a specialized planning engine for users attending local experiences with specific accessibility needs. It helps users manage privacy through minimum necessary disclosure principles while ensuring logistical readiness. Use `get_confirmation_questions` to verify venue features, `generate_contact_sequence` to schedule communications, and `calculate_decision_point` to evaluate if a venue meets requirements. It also includes `plan_day_of_support` for arrival logistics and `get_feedback_route` for post-experience reporting.


## Available Tools (5)
- **generate_contact_sequence**: Creates a schedule of communications to ensure the provider is prepared
- **get_confirmation_questions**: Generates a tailored set of questions to ask the experience provider to verify accessibility
- **get_feedback_route**: Generates a way for the user to report the experience
- **plan_day_of_support**: Designs the immediate logistics for the day the experience takes place
- **calculate_decision_point**: Provides a structured framework for the user to decide whether to attend based on the responses received


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessibility Confirmation Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to check if a museum has step-free access. I want to keep my details private."

**🤖 AI Agent:**
> I will use `get_confirmation_questions` with low disclosure to ask about ramps and elevators at the museum.

---

**👤 You:**
> "Help me plan my arrival for a concert tomorrow using a wheelchair accessible vehicle."

**🤖 AI Agent:**
> I will use `plan_day_of_support` to create an arrival protocol and assistance handover plan for your concert.

---

**👤 You:**
> "The venue said they only have stairs. I need step-free access. Should I go?"

**🤖 AI Agent:**
> Based on your requirement for step-free access and the venue's confirmation of only having stairs, the recommendation is to decline the experience.


## ❓ FAQ

**Q: How does this tool protect my privacy?**
The tool uses a Minimum Necessary Disclosure principle. When using `get_confirmation_questions` with a low disclosure level, it focuses on environmental attributes rather than personal medical details.

**Q: Can I use this to plan my arrival?**
Yes, you can use `plan_day_of_support` to design arrival protocols, assistance handovers, and contingency contacts based on your specific needs.

**Q: What happens if the venue doesn't meet my needs?**
You can use `calculate_decision_point` to evaluate the venue's responses against your requirements to decide whether to attend or decline.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessibility-confirmation-planner](https://vinkius.com/en/ai-agent-connect/accessibility-confirmation-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessibility Confirmation Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessibility-confirmation-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessibility Confirmation Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessibility-confirmation-planner": {
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
