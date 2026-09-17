# Box Jump Height Recommender MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/box-jump-height-recommender)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Safe and effective box jump height recommendations based on explosive power and experience.

## Description
This MCP server provides specialized guidance for athletes looking to optimize their plyometric training. By analyzing your standing vertical jump and physical profile, the server uses `get_recommended_height` to suggest the safest optimal box height. It also provides structured training paths via `generate_progression_plan`, identifies specific risks through `get_safety_considerations`, and suggests suitable movements with `get_alternative_exercises` if a full box jump is not yet appropriate for your experience level.


## Available Tools (4)
- **generate_progression_plan**: Creates a structured multi-stage plan to help the user increase their box jump height over time
- **get_alternative_exercises**: Suggests movements that build the necessary components of the box jump if the user cannot perform it safely
- **get_recommended_height**: Determines the single most appropriate box height for a user's current profile
- **get_safety_considerations**: Provides specific physiological and environmental warnings tailored to the user's profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Box Jump Height Recommender** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a 50cm vertical jump, I am 180cm tall, I am a beginner, and my goal is stability. What height should I use?"

**🤖 AI Agent:**
> Based on your profile, the recommended box height is 35cm to ensure safe landing mechanics.

---

**👤 You:**
> "I am an advanced athlete with a 65cm vertical jump. I want to increase my height by 10cm. Can you give me a plan?"

**🤖 AI Agent:**
> Your progression plan will consist of 4 stages over 8 weeks, starting with incremental height increases to build reactive power.

---

**👤 You:**
> "What are the safety risks for an intermediate athlete focusing on power?"

**🤖 AI Agent:**
> For intermediate athletes focusing on power, the primary risk is tendon overload; focus on explosive takeoff and controlled landings.


## ❓ FAQ

**Q: How is the recommended height calculated?**
The height is determined by your standing vertical jump, adjusted by a safety buffer that accounts for your experience level and training goals.

**Q: Can I use this for beginner training?**
Yes, the tool specifically includes safety buffers and alternative exercises for beginners to ensure proper landing mechanics.

**Q: What if I cannot jump onto a box safely?**
You can use `get_alternative_exercises` to find movements that build the necessary explosive power and stability for future box jumps.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/box-jump-height-recommender](https://vinkius.com/en/ai-agent-connect/box-jump-height-recommender)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Box Jump Height Recommender** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `box-jump-height-recommender` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Box Jump Height Recommender** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "box-jump-height-recommender": {
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
