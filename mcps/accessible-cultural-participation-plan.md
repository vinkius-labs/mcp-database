# Accessible Cultural Participation Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-cultural-participation-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [accessibility](../categories/accessibility.md)

Evaluates cultural activity feasibility and generates personalized engagement strategies for accessibility.

## Description
This MCP server provides a comprehensive framework for assessing if cultural events are accessible to users with specific needs. It uses `evaluate_participation` to determine feasibility, `generate_request_plan` to bridge the gap between user requirements and venue provisions, `create_engagement_plan` to build a personalized visit roadmap, and `get_feedback_route` to capture post-visit experiences. It acts as a bridge between individual accessibility requirements and venue capabilities.


## Available Tools (4)
- **get_feedback_route**: Provide a structured way to report on the experience
- **create_engagement_plan**: Produce a personalized step-by-step guide for the user during the event
- **evaluate_participation**: Determine if a cultural activity is feasible based on user needs and venue details
- **generate_request_plan**: Identify necessary requests and confirmation items for the venue


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Cultural Participation Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to go to the Modern Art Gallery. The venue has ramps and a quiet room. I need low sensory stimulation and wheelchair access. Is this feasible?"

**🤖 AI Agent:**
> Yes, the Modern Art Gallery is feasible for your needs. The presence of ramps supports your mobility requirements, and the quiet room addresses your sensory needs for low stimulation.

---

**👤 You:**
> "The venue has ramps but no sensory kits. I have high sensory needs. What should I ask them?"

**🤖 AI Agent:**
> You should request a sensory kit or ask if they can provide a quiet space for breaks. You should also confirm if they have staff trained in sensory accommodations.

---

**👤 You:**
> "I just finished my visit to the Jazz Festival. It was a great experience and all my needs were met."

**🤖 AI Agent:**
> I'm glad to hear the Jazz Festival was a success! I have prepared a feedback route focusing on the sensory environment and the effectiveness of the staff interactions to help improve future visits.


## ❓ FAQ

**Q: How does the tool determine if an event is accessible?**
The `evaluate_participation` tool compares the user's specific mobility, sensory, and cognitive requirements against the documented provisions of the venue to identify any gaps or risks.

**Q: Can I get a list of things to ask the venue?**
Yes, the `generate_request_plan` tool identifies the specific accommodations needed and provides a list of formal requests and confirmation items for the venue staff.

**Q: What happens after the cultural event is over?**
You can use `get_feedback_route` to receive a customized set of questions to evaluate how well the accommodations worked and if your participation goals were met.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-cultural-participation-plan](https://vinkius.com/en/ai-agent-connect/accessible-cultural-participation-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Cultural Participation Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-cultural-participation-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Cultural Participation Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-cultural-participation-plan": {
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
