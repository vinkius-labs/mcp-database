# Local Food & Culture Experience Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/local-food-culture-experience-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Plan cohesive cultural dining itineraries by synthesizing user preferences, dietary needs, and venue constraints.

## Description
This MCP server acts as a specialized planning engine for cultural dining. It connects AI agents to a suite of tools designed to evaluate venue suitability, select optimal dining locations, and generate detailed logistics. By using `analyze_experience_suitability`, agents can verify if a venue meets hard constraints like dietary needs or access requirements. The `select_primary_and_alternate` tool helps pick the best fit from multiple options, while `generate_logistics_plan` provides arrival details and reservation actions. It also includes `validate_privacy_compliance` to ensure user data is handled according to their disclosure boundaries.


## Available Tools (4)
- **analyze_experience_suitability**: Determines if a specific venue is a valid match based on user constraints and venue rules
- **generate_logistics_plan**: Creates the practical execution details for a chosen experience
- **select_primary_and_alternate**: Evaluates a list of potential venues to pick the best fit and a secondary fallback
- **validate_privacy_compliance**: Ensures that the planning process respects the user's willingness to disclose information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Local Food & Culture Experience Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to find a place for a group of 4 with vegan requirements and wheelchair access. Here are two options: [Option A: Vegan bistro, stairs only] [Option B: Garden cafe, ramp access, vegan friendly]."

**🤖 AI Agent:**
> The primary choice is the Garden cafe because it meets both the vegan dietary requirement and the wheelchair access need. The bistro is unsuitable due to the stairs.

---

**👤 You:**
> "Help me plan the arrival for our dinner at The Golden Grill at 7 PM. We are a group of 3 and need to arrive by 6:45 PM."

**🤖 AI Agent:**
> To arrive at The Golden Grill by 6:45 PM, please depart by 6:30 PM to account for travel. You should confirm your reservation via their website before leaving. I have notified the group of the 6:45 PM arrival time.

---

**👤 You:**
> "Is this venue suitable? Venue: Traditional Sushi House. Rules: No substitutions for allergies. User: I have a severe peanut allergy."

**🤖 AI Agent:**
> The venue is unsuitable because it cannot accommodate your mandatory peanut allergy disclosure due to its strict no-substitution policy.


## ❓ FAQ

**Q: How does the tool handle dietary restrictions?**
The `analyze_experience_suitability` tool checks if a venue can accommodate mandatory dietary disclosures. If a venue cannot meet a hard constraint, it is flagged as unsuitable.

**Q: Can I plan the logistics for my group?**
Yes, you can use `generate_logistics_plan` to create arrival plans, reservation steps, and communication summaries for all participants.

**Q: How is user privacy protected?**
The `validate_privacy_compliance` tool ensures that the planning process only uses information the user has explicitly chosen to disclose to the venue.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/local-food-culture-experience-planner](https://vinkius.com/en/ai-agent-connect/local-food-culture-experience-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Local Food & Culture Experience Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `local-food-culture-experience-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Local Food & Culture Experience Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "local-food-culture-experience-planner": {
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
