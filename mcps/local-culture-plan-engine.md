# Local Culture Plan Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/local-culture-plan-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Generates feasible visit sequences and logistics for cultural outings.

## Description
This MCP server provides specialized planning tools to coordinate cultural visits. It calculates valid visit sequences using `get_feasible_sequence`, identifies necessary preparatory tasks with `get_advance_actions`, defines meetup protocols via `get_meeting_protocol`, and establishes movement commitments through `get_transition_plan`. It ensures all plans respect venue opening hours, ticket constraints, accessibility needs, and time ceilings.


## Available Tools (4)
- **get_feasible_sequence**: Find a valid order of visits that fits within the user's constraints
- **get_meeting_protocol**: Define how and where the group should gather
- **get_transition_plan**: Define the specific movement commitments between each stop
- **get_advance_actions**: Identify specific preparatory tasks needed before the group departs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Local Culture Plan Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a visit to the Museum and the Art Gallery with a 3-hour limit and wheelchair access."

**🤖 AI Agent:**
> Your visit sequence is: 1. Museum (10:00 - 11:30), 2. Art Gallery (12:00 - 13:00). Total time: 180 minutes.

---

**👤 You:**
> "What should I do to prepare for my visit to the Botanical Gardens?"

**🤖 AI Agent:**
> You should confirm your entry ticket and verify the availability of the accessible walking paths.

---

**👤 You:**
> "Where should we meet for our museum visit?"

**🤖 AI Agent:**
> The group should meet at the Museum main entrance at 09:45.


## ❓ FAQ

**Q: How does the tool handle accessibility?**
The `get_feasible_sequence` tool filters all possible routes and venues to ensure they meet the specific accessibility requirements provided by the user.

**Q: Can I plan a trip with a strict time limit?**
Yes, you can provide a time ceiling, and the `get_feasible_sequence` tool will only return sequences that fit within that duration.

**Q: What if my planned route is too long?**
The `get_feasible_sequence` tool can provide a reduction option, which is a specific recommendation to remove one venue to make the plan feasible.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/local-culture-plan-engine](https://vinkius.com/en/ai-agent-connect/local-culture-plan-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Local Culture Plan Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `local-culture-plan-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Local Culture Plan Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "local-culture-plan-engine": {
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
