# Care Provider Interview Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/care-provider-interview-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

A decision-support system for evaluating care provider candidates against family requirements.

## Description
This MCP server provides a suite of tools to help families select the right care provider. It uses a weighted selection rubric and mandatory criteria to evaluate candidates. You can use `generate_interview_questions` to create tailored questions, `compare_candidates` to rank multiple profiles, `generate_reference_check_tasks` to build verification checklists, and `create_onboarding_brief` to generate a final selection summary.


## Available Tools (4)
- **generate_interview_questions**: Creates a customized list of questions to ask a candidate
- **compare_candidates**: Ranks multiple candidates against weighted rubric and mandatory criteria
- **create_onboarding_brief**: Generates a final decision summary for the selected provider
- **generate_reference_check_tasks**: Produces a checklist of items to verify with references


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Care Provider Interview Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare these two candidates: Alice (Score: 85, Mandatory: Pass) and Bob (Score: 90, Mandatory: Fail)."

**🤖 AI Agent:**
> Alice is the qualified candidate. Although Bob has a higher score, he failed the mandatory criteria and is therefore disqualified.

---

**👤 You:**
> "Generate interview questions for a candidate for meal prep and light cleaning."

**🤖 AI Agent:**
> 1. Can you describe your experience with meal preparation for specific dietary needs? 2. How do you manage your schedule to ensure light cleaning tasks are completed daily?

---

**👤 You:**
> "Create a reference check task for a candidate who claims to have 5 years of experience."

**🤖 AI Agent:**
> Verify the candidate's employment history with previous employers to confirm they have completed at least 5 years of professional caregiving experience.


## ❓ FAQ

**Q: How does the candidate ranking work?**
The system uses a weighted rubric where you assign importance to different factors. It also enforces mandatory criteria; if a candidate fails a mandatory requirement, they are automatically disqualified.

**Q: Can I generate specific questions for a candidate?**
Yes, you can use the `generate_interview_questions` tool to create a customized list of questions based on the required tasks and the candidate's profile.

**Q: What is included in the onboarding brief?**
The `create_onboarding_brief` tool produces a structured summary that includes the selection justification, a fit summary, and identified risks to help you move forward with the provider.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/care-provider-interview-planner](https://vinkius.com/en/ai-agent-connect/care-provider-interview-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Care Provider Interview Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `care-provider-interview-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Care Provider Interview Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "care-provider-interview-planner": {
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
