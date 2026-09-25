# Care Provider Onboarding Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/care-provider-onboarding-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Orchestrates structured onboarding for care providers through staged orientation and sign-off gates.

## Description
This MCP server manages the complete onboarding lifecycle for care providers. It transforms raw household data and provider details into actionable artifacts. Using tools like `get_day_one_briefing` and `generate_first_week_schedule`, it ensures providers receive essential safety rules and structured timelines. The system implements staged orientation (Introductory, Supervised, Autonomous) with mandatory sign-off gates. It also facilitates consistent communication via `create_handoff_template` and manages progress reviews with `prepare_review_meeting_agenda`.


## Available Tools (4)
- **generate_first_week_schedule**: 
- **create_handoff_template**: 
- **get_day_one_briefing**: 
- **prepare_review_meeting_agenda**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Care Provider Onboarding Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me the day-one briefing for provider P123 in household H456."

**🤖 AI Agent:**
> Here is your Day One Briefing: Your primary contact is Sarah (Emergency: 555-0199). Safety Rule: Do not enter the basement without supervision. Immediate Routine: Breakfast service begins at 8:00 AM.

---

**👤 You:**
> "Generate a first-week schedule for provider P123 in household H456 starting on 2024-11-01."

**🤖 AI Agent:**
> Your schedule for the week of Nov 1st is ready. Day 1: Observation. Day 2: Supervised meal prep. End of Day 2: Sign-off gate for 'Introductory' stage. Day 3-5: Active duty with oversight.

---

**👤 You:**
> "Create a digital-log handoff template for provider P123."

**🤖 AI Agent:**
> Your digital-log template is ready. It includes sections for: Completed Tasks, Medication Administration, Household Observations, and Next Shift Notes.


## ❓ FAQ

**Q: How does the onboarding process ensure safety?**
Safety is maintained through `get_day_one_briefing`, which prioritizes access limits and safety-critical rules, and through staged sign-off gates that prevent moving to higher responsibility without verified competency.

**Q: Can I customize the daily reporting format?**
Yes, you can use `create_handoff_template` to generate standardized communication tools based on the household's preferred reporting method, such as digital logs or written notes.

**Q: What happens during a final sign-off?**
Using `prepare_review_meeting_agenda` with the 'final-sign-off' type will produce a plan that includes all pending checklist items required to transition the provider to full autonomy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/care-provider-onboarding-plan](https://vinkius.com/en/ai-agent-connect/care-provider-onboarding-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Care Provider Onboarding Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `care-provider-onboarding-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Care Provider Onboarding Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "care-provider-onboarding-plan": {
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
