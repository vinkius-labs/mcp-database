# Competition Anxiety Management for Surfers MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/competition-anxiety-management-for-surfers)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [performance](../categories/performance.md)

Tailored anxiety mitigation and breathing protocols for surfers.

## Description
This MCP server provides specialized tools to help surfers manage performance-inhibiting anxiety. By analyzing physiological and cognitive symptoms, the server uses `get_anxiety_assessment` to determine anxiety intensity. It then provides targeted physiological regulation via `generate_breathing_protocol`, constructs structured pre-competition sequences with `create_pre_heat_routine`, and develops long-term mental strategies through `generate_management_plan`.


## Available Tools (4)
- **create_pre_heat_routine**: Construct a timed sequence of actions to prepare the surfer for the heat
- **generate_breathing_protocol**: Provide a specific respiratory technique to regulate the nervous system
- **generate_management_plan**: Provide a comprehensive long-term strategy for managing competition anxiety
- **get_anxiety_assessment**: Evaluate the current state of a surfer's anxiety based on reported symptoms and experience


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Competition Anxiety Management for Surfers** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I'm feeling nausea and trembling before my first local contest. I'm a novice."

**🤖 AI Agent:**
> Your assessment score is 75, indicating high somatic anxiety. I recommend the Box Breathing technique for 5 minutes to stabilize your heart rate.

---

**👤 You:**
> "I have racing thoughts and fear of failure during professional heats. I use visualization."

**🤖 AI Agent:**
> Your assessment score is 60 with a cognitive driver. We will integrate your visualization strategy into a 10-minute pre-heat routine.

---

**👤 You:**
> "Give me a long-term plan for managing racing thoughts as an intermediate surfer."

**🤖 AI Agent:**
> Your core strategy is cognitive reframing. Recommended practices include daily mindfulness and weekly breathing drills. Review this plan monthly.


## ❓ FAQ

**Q: How does the assessment work?**
The `get_anxiety_assessment` tool evaluates your reported symptoms and competitive experience to determine your anxiety intensity and primary driver.

**Q: Can I get a routine for right before a heat?**
Yes, you can use `create_pre_heat_routine` to generate a timed sequence of actions, including breathing and coping strategies, to prepare you for competition.

**Q: What kind of breathing techniques are provided?**
The `generate_breathing_protocol` tool provides specific respiratory techniques tailored to whether your anxiety is somatic (physical) or cognitive (mental).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/competition-anxiety-management-for-surfers](https://vinkius.com/en/ai-agent-connect/competition-anxiety-management-for-surfers)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Competition Anxiety Management for Surfers** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `competition-anxiety-management-for-surfers` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Competition Anxiety Management for Surfers** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "competition-anxiety-management-for-surfers": {
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
