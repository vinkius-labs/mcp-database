# Local Experience Group Agreement MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/local-experience-group-agreement)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate structured group agreements, commitment timelines, and logistical frameworks for shared local activities.

## Description
This MCP server provides a complete logistical framework for organizing group activities. It allows AI agents to generate formal group agreements that include commitment timelines, individual responsibilities, and clear withdrawal processes. By using tools like `generate_group_agreement`, agents can ensure all participants align on spending limits, accessibility needs, and decision-making rules (such as Unanimous or Majority consensus). It also includes tools to `validate_participation_status` and `verify_cancellation_compliance` to manage group dynamics effectively.


## Available Tools (4)
- **calculate_individual_responsibility_load**: Distributes specific duties among participants to ensure the activity is organized
- **generate_group_agreement**: Creates the comprehensive formal agreement and logistical package for a group activity
- **validate_participation_status**: Checks if a specific participant is eligible to join based on the current agreement and their stated availability
- **verify_cancellation_compliance**: Determines if a requested withdrawal is within the agreed-upon boundaries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Local Experience Group Agreement** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a group agreement for Alice, Bob, and Charlie for a hiking trip this Saturday with a $50 limit per person."

**🤖 AI Agent:**
> Group Agreement: Hiking Trip. Participants: Alice, Bob, Charlie. Availability: This Saturday. Spending Limit: $50. Decision Rule: Majority. Timeline: Confirmation by Friday, Payment by Saturday morning. Responsibilities: Alice (Navigation), Bob (First Aid), Charlie (Snacks).

---

**👤 You:**
> "Is Dave eligible to join the group if the activity is on Friday and he is only available on Saturday?"

**🤖 AI Agent:**
> No, Dave is not eligible because his availability does not overlap with the planned activity window.

---

**👤 You:**
> "Can I cancel my participation for the dinner tonight without a penalty if the cancellation window is 24 hours?"

**🤖 AI Agent:**
> No, the request was made within the 24-hour window, so a penalty may apply according to the agreement.


## ❓ FAQ

**Q: How does the agreement handle decision making?**
The agreement uses the specified `decisionRule` (such as Unanimous, Majority, or LeadDecider) to define how the group reaches consensus on future choices.

**Q: Can I check if a participant is available for the activity?**
Yes, you can use the `validate_participation_status` tool to check if a person's availability window overlaps with the planned activity window.

**Q: What happens if someone needs to withdraw from the group?**
The `verify_cancellation_compliance` tool determines if a withdrawal is within the agreed `cancellationWindow` to avoid penalties.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/local-experience-group-agreement](https://vinkius.com/en/ai-agent-connect/local-experience-group-agreement)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Local Experience Group Agreement** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `local-experience-group-agreement` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Local Experience Group Agreement** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "local-experience-group-agreement": {
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
