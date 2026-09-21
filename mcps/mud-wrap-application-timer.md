# Mud Wrap Application Timer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/mud-wrap-application-timer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [wellness](../categories/wellness.md)

Calculates precise mud wrap protocols, safety limits, and post-treatment care.

## Description
A specialized engine for professional spa treatments. It uses `calculate_wrap_protocol` to determine application thickness and duration, `get_skin_safety_limit` to ensure client safety, `get_removal_instructions` for effective cleanup, and `get_post_treatment_regimen` for skin recovery. This tool connects AI agents to professional mud wrap protocols for detox, slimming, and relaxation goals.


## Available Tools (4)
- **calculate_wrap_protocol**: Determines the fundamental application parameters for a mud wrap session
- **get_post_treatment_regimen**: Provides a set of recovery instructions to ensure skin stability after the wrap
- **get_removal_instructions**: Provides specific physical instructions for removing the wrap safely and effectively
- **get_skin_safety_limit**: Validates if a requested treatment duration is safe for a specific skin type and mud combination


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mud Wrap Application Timer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a protocol for a detox wrap using Seaweed mud on the abdomen for a client with dry skin."

**🤖 AI Agent:**
> The protocol for Seaweed mud on the abdomen for dry skin (detox) requires a thickness of 5mm and a duration of 30 minutes. Removal should be done via Warm Towel, followed by deep hydration.

---

**👤 You:**
> "Is a 45-minute Bentonite wrap safe for sensitive skin?"

**🤖 AI Agent:**
> No, for sensitive skin using Bentonite mud, the maximum safe duration is 20 minutes to prevent irritation.

---

**👤 You:**
> "What are the post-treatment steps for a slimming wrap on normal skin?"

**🤖 AI Agent:**
> After a slimming wrap on normal skin, prioritize fluid replenishment and use a lightweight moisturizer. Avoid direct sun exposure for 24 hours.


## ❓ FAQ

**Q: How does the tool ensure skin safety?**
The `get_skin_safety_limit` tool validates requested durations against specific skin types and mud compositions to prevent irritation.

**Q: Can I use this for different therapeutic goals?**
Yes, the engine supports specific protocols for detox, slimming, and relaxation goals.

**Q: What information is needed to start a protocol?**
You need to provide the mud type, the body areas being treated, the client's skin type, and the therapeutic goal.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/mud-wrap-application-timer](https://vinkius.com/en/ai-agent-connect/mud-wrap-application-timer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mud Wrap Application Timer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mud-wrap-application-timer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mud Wrap Application Timer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mud-wrap-application-timer": {
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
