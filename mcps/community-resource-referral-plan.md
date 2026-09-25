# Community Resource Referral Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/community-resource-referral-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [decision-engine](../categories/decision-engine.md)

Transforms non-clinical needs into actionable referral sequences, communication scripts, and follow-up schedules.

## Description
This MCP server acts as a decision engine for community support. It processes user needs, eligibility constraints, and contact priorities to generate a complete referral roadmap. Use `identify_eligible_resources` to filter available support, `generate_referral_sequence` to build a timeline, `prepare_communication_package` for tailored scripts, and `create_followup_schedule` to ensure successful outcomes.


## Available Tools (4)
- **create_followup_schedule**: Generates a timeline of touchpoints to ensure the referral process is successfully completed
- **generate_referral_sequence**: Organizes the eligible resources into a prioritized chronological plan of action
- **identify_eligible_resources**: Determines which resources from the approved list meet the user's specific eligibility and constraint profile
- **prepare_communication_package**: Creates the specific documentation and verbal templates needed to execute the referral


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Community Resource Referral Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need food assistance for a family of four in Chicago. They have no car and need help immediately."

**🤖 AI Agent:**
> I have identified two food pantries in Chicago that offer transit-accessible locations and meet your household size requirements. I will now generate a prioritized referral sequence and contact scripts for you.

---

**👤 You:**
> "Create a follow-up plan for a housing referral with weekly check-ins."

**🤖 AI Agent:**
> The follow-up calendar has been generated with weekly check-ins starting from your referral deadline to ensure the housing application is progressing.

---

**👤 You:**
> "What documents do I need for the utility assistance program?"

**🤖 AI Agent:**
> The communication package includes a list of required documents, such as proof of residency and recent utility bills, to present to the provider.


## ❓ FAQ

**Q: How does the server determine which resources are suitable?**
The `identify_eligible_resources` tool matches user constraints like income, residency, and transport availability against the provided resource list.

**Q: Can I generate scripts in different languages?**
Yes, the `prepare_communication_package` tool generates contact scripts in the user's preferred language.

**Q: How are the referral steps prioritized?**
The `generate_referral_sequence` tool organizes steps based on user-provided `contactOrderRules`, such as prioritizing emergency needs over long-term stability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/community-resource-referral-plan](https://vinkius.com/en/ai-agent-connect/community-resource-referral-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Community Resource Referral Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `community-resource-referral-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Community Resource Referral Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "community-resource-referral-plan": {
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
