# Grounding & Earthing Duration Guide MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/grounding-earthing-duration-guide)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Personalized grounding practice schedules based on health goals and contact methods.

## Description
This MCP server provides scientific guidance for earthing practices. It helps users determine the ideal duration, optimal time of day, and weekly frequency for grounding sessions. By using tools like `get_recommended_duration` and `get_optimal_timing`, users can align their physical contact with the Earth--whether barefoot, using a mat, or at the beach--to meet specific physiological objectives like stress reduction or sleep optimization.


## Available Tools (4)
- **get_frequency_plan**: Suggests how many times per week the user should practice
- **get_method_suitability**: Evaluates if a chosen grounding method is appropriate for a specific goal
- **get_optimal_timing**: Suggests the best time of day to perform the grounding session
- **get_recommended_duration**: Determines the specific time length for a single grounding session


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Grounding & Earthing Duration Guide** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to reduce stress. I am barefoot on grass and have 20 minutes. How long should I stay?"

**🤖 AI Agent:**
> For stress reduction via barefoot contact, 20 minutes is a sufficient duration to begin feeling the physiological benefits.

---

**👤 You:**
> "What is the best time of day for sleep optimization?"

**🤖 AI Agent:**
> Evening grounding is recommended for sleep optimization to help support melatonin production.

---

**👤 You:**
> "How many times a week should I ground if I want to manage inflammation with 30-minute sessions?"

**🤖 AI Agent:**
> To manage inflammation with 30-minute sessions, you should practice 5 to 7 days per week for consistent physiological impact.


## ❓ FAQ

**Q: How do I know how long I should ground?**
You can use the `get_recommended_duration` tool to calculate the ideal session length based on your specific health goal and the method of contact you are using.

**Q: Can I use this for sleep improvement?**
Yes. By using `get_optimal_timing` with the sleep optimization goal, you can find the best time of day to ground to support your circadian rhythm.

**Q: Is beach grounding better than using a mat?**
You can evaluate this by using the `get_method_suitability` tool, which compares different grounding types for your specific health objectives.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/grounding-earthing-duration-guide](https://vinkius.com/en/ai-agent-connect/grounding-earthing-duration-guide)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Grounding & Earthing Duration Guide** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `grounding-earthing-duration-guide` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Grounding & Earthing Duration Guide** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "grounding-earthing-duration-guide": {
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
