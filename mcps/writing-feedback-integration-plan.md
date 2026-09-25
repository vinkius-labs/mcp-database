# Writing Feedback Integration Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/writing-feedback-integration-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A strategic decision engine that parses manuscript feedback against user-defined constraints to generate actionable revision roadmaps.

## Description
This MCP server provides a suite of tools to manage the complex process of manuscript revision. It uses a decision framework to categorize feedback into Accept, Adapt, or Defer based on your specific Acceptance Criteria and Non-negotiable Voice. Key tools include `analyze_feedback_decisions` for categorization, `generate_revision_brief` for task synthesis, `compose_reviewer_followup` for clarifying intent, `create_implementation_roadmap` for sequencing tasks, and `generate_post_revision_review_plan` for final verification.


## Available Tools (5)
- **analyze_feedback_decisions**: Categorize feedback into accept, adapt, or defer based on constraints
- **generate_revision_brief**: Transform decisions into a cohesive set of instructions
- **compose_reviewer_followup**: Identify gaps in feedback to generate follow-up questions
- **create_implementation_roadmap**: Sequence revision tasks into a logical order
- **generate_post_revision_review_plan**: Provide a checklist to verify the revision met goals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Writing Feedback Integration Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this feedback: 'The protagonist's tone is too aggressive in chapter 3.' against my criteria: 'Maintain a polite, professional tone at all times.'"

**🤖 AI Agent:**
> Decision: Adapt. Reasoning: The feedback identifies a tonal issue that conflicts with the requirement for a polite tone. The task is to soften the dialogue in chapter 3 to ensure it remains professional while preserving the character's core personality.

---

**👤 You:**
> "Generate a revision brief for these decisions: [{"commentId": "1", "decision": "accept", "reasoning": "Fixes a typo."}, {"commentId": "2", "decision": "adapt", "reasoning": "Adjusts pacing without changing plot."}]. Goal: Improve readability."

**🤖 AI Agent:**
> Summary: Focus on improving readability through minor corrections and pacing adjustments. Tasks: 1. Correct identified typographical errors. 2. Adjust sentence pacing in key sections to improve flow.

---

**👤 You:**
> "Create a roadmap for these decisions: [{"commentId": "1", "decision": "accept", "reasoning": "Structural change needed."}]. Window: 2 hours."

**🤖 AI Agent:**
> Sequence: 1. Implement the structural changes to the chapter outline. 2. Re-align subsequent scene transitions. Complexity: High.


## ❓ FAQ

**Q: How does the tool decide to 'Adapt' feedback?**
Feedback is marked as 'Adapt' when it offers useful improvements but would violate your defined Non-negotiable Voice or Acceptance Criteria if implemented directly. The tool suggests modifications to align the suggestion with your intent.

**Q: What is the purpose of the implementation roadmap?**
The `create_implementation_roadmap` tool sequences your revision tasks using a foundation-first approach, ensuring structural and logical changes are addressed before micro-level stylistic adjustments.

**Q: Can I use this for different types of writing projects?**
Yes, the engine is designed to be flexible. By defining your own Acceptance Criteria and Revision Window, you can apply this logic to novels, technical manuscripts, or academic papers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/writing-feedback-integration-plan](https://vinkius.com/en/ai-agent-connect/writing-feedback-integration-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Writing Feedback Integration Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `writing-feedback-integration-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Writing Feedback Integration Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "writing-feedback-integration-plan": {
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
