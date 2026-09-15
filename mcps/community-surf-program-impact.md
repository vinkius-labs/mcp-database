# Community Surf Program Impact MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/community-surf-program-impact)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analysis](../categories/data-analysis.md)

Quantifies social, physical, and community-level impact of surf-based outreach programs.

## Description
This MCP server provides a specialized assessment engine to measure the influence of surf-based community programs. It uses standardized methodologies to calculate social impact, health outcomes, and community benefits. Using tools like `get_participant_impact_summary`, `analyze_program_effectiveness`, `compare_demographic_outcomes`, and `assess_community_benefit_index`, AI agents can evaluate individual progress, program-wide success, demographic equity, and broader community-level advantages.


## Available Tools (4)
- **analyze_program_effectiveness**: Evaluates the overall success of a specific surf program across all its participants
- **get_participant_impact_summary**: Provides a high-level overview of the impact achieved for a specific participant
- **assess_community_benefit_index**: Quantifies the broader community-level advantages derived from the surf program
- **compare_demographic_outcomes**: Analyzes how impact differs across various demographic groups to identify equity in program delivery


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Community Surf Program Impact** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the impact summary for participant P123?"

**🤖 AI Agent:**
> Participant P123 has a social impact score of 85 and a health impact score of 78, with a high level of engagement.

---

**👤 You:**
> "How effective was program PRG-001?"

**🤖 AI Agent:**
> Program PRG-001 had 50 participants with an average social impact of 72 and an average health impact of 65, resulting in a High effectiveness rating.

---

**👤 You:**
> "Show me the community benefits for program PRG-001."

**🤖 AI Agent:**
> Program PRG-001 achieved a social capital index of 75 and a community health benefit score of 68.


## ❓ FAQ

**Q: How does the server measure social impact?**
Social impact is measured by analyzing changes in interpersonal relationships, social cohesion, and the individual sense of community connection through `get_participant_impact_summary` and other analysis tools.

**Q: Can I analyze equity across different groups?**
Yes, you can use `compare_demographic_outcomes` to identify how impact differs across various demographic categories, ensuring equitable program delivery.

**Q: Does it include environmental benefits?**
Yes, by using `assess_community_benefit_index` with the environmental metrics flag enabled, you can retrieve scores for coastal ecosystem benefits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/community-surf-program-impact](https://vinkius.com/en/ai-agent-connect/community-surf-program-impact)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Community Surf Program Impact** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `community-surf-program-impact` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Community Surf Program Impact** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "community-surf-program-impact": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
