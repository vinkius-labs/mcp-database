# Promotion Readiness Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/promotion-readiness-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Maps achievements, skills, and feedback against promotion criteria to identify evidence gaps and projected timelines.

## Description
The Promotion Readiness Tracker connects AI agents to your professional development data. By using tools like `get_readiness_gap_analysis` and `get_promotion_timeline`, an agent can identify exactly which competencies are missing for a target role and estimate when you will be ready for your next career move. It provides a clear view of your professional standing through `list_employee_evidence_summary` and `evaluate_skill_alignment`.


## Available Tools (4)
- **evaluate_skill_alignment**: Checks how well the user's current skill set matches the requirements of the next level
- **list_employee_evidence_summary**: Provides a structured overview of all currently documented evidence
- **get_promotion_timeline**: Predicts the estimated timeframe for promotion based on current progress
- **get_readiness_gap_analysis**: Identifies specific areas where the user lacks the evidence required for a target promotion


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Promotion Readiness Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What am I missing to be promoted to Senior level?"

**🤖 AI Agent:**
> To reach the Senior level, you currently lack evidence in 'Strategic Planning' and 'Mentorship'. You have satisfied 65% of the required criteria.

---

**👤 You:**
> "When will I likely be ready for a Mid-level role?"

**🤖 AI Agent:**
> Based on your current progress, you are estimated to be ready for a Mid-level role in approximately 4 months.

---

**👤 You:**
> "Show me a summary of my current professional evidence."

**🤖 AI Agent:**
> Your current profile includes 5 verified achievements, 12 documented skills, and 3 pieces of positive peer feedback.


## ❓ FAQ

**Q: How does the tracker identify gaps?**
It uses `get_readiness_gap_analysis` to compare your documented achievements and skills against the standardized requirements for your target role level.

**Q: Can I get an estimate of my promotion date?**
Yes, the `get_promotion_timeline` tool calculates an estimated timeframe based on your current progress and the velocity of new evidence being added.

**Q: What kind of evidence is used?**
The system aggregates achievements, technical and soft skills, and qualitative feedback to build a complete profile of your readiness.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/promotion-readiness-tracker](https://vinkius.com/en/ai-agent-connect/promotion-readiness-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Promotion Readiness Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `promotion-readiness-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Promotion Readiness Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "promotion-readiness-tracker": {
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
