# Accessible Event Accommodation Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-event-accommodation-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates privacy-respecting accommodation requests based on event policies.

## Description
This MCP server helps users navigate accessibility requests by applying the Minimum-Disclosure Rule. It uses `analyze_policy_and_request` to create optimized requests, `validate_disclosure_compliance` to ensure privacy, `calculate_submission_urgency` to track deadlines, and `generate_escalation_strategy` to provide clear contact paths. It acts as a bridge between attendee needs and organizational requirements.


## Available Tools (4)
- **analyze_policy_and_request**: Evaluates the intersection between the organizer's policy and the user's specific needs
- **calculate_submission_urgency**: Determines how much time remains before the deadline
- **generate_escalation_strategy**: Builds a structured hierarchy of contact points if the primary request is not acknowledged
- **validate_disclosure_compliance**: Verifies if a drafted request adheres to the Minimum-Disclosure Rule


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Event Accommodation Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to request a sign language interpreter for an in-person conference. The policy says to email accessibility@event.com by Oct 1st. Here is the policy: [Policy Text]. I can provide a doctor's note if needed."

**🤖 AI Agent:**
> Request: 'I am writing to request a sign language interpreter for the upcoming in-person conference. Please let me know the next steps for this accommodation.'
Questions: Would you like to include the specific date of the conference?
Timeline: You should receive a response by the October 1st deadline.
Escalation: If no response is received, contact the Event Coordinator.

---

**👤 You:**
> "How much time do I have left to submit my request for the workshop on Dec 15th? The deadline is Dec 10th and today is Dec 8th."

**🤖 AI Agent:**
> You have 2 days remaining. Your urgency level is Critical.

---

**👤 You:**
> "Check if this request is okay: 'I need a ramp because I use a wheelchair. My medical history shows I have mobility issues.' Policy: 'Requests must state the required accommodation.'"

**🤖 AI Agent:**
> The request is non-compliant. It includes unnecessary medical history that is not required by the policy. You should only state the need for a ramp.


## ❓ FAQ

**Q: How does this tool protect my privacy?**
The tool uses the `validate_disclosure_compliance` function to ensure that only the essential information required by the organizer's policy is included in your request, adhering to the Minimum-Disclosure Rule.

**Q: Can I use this for virtual events?**
Yes, by providing the event format in the `analyze_policy_and_request` tool, the generated plan will account for the specific needs of virtual, in-person, or hybrid settings.

**Q: What happens if my request is ignored?**
The `generate_escalation_strategy` tool builds a structured hierarchy of contact points based on the organizer's policy to guide your next steps.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-event-accommodation-planner](https://vinkius.com/en/ai-agent-connect/accessible-event-accommodation-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Event Accommodation Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-event-accommodation-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Event Accommodation Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-event-accommodation-planner": {
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
