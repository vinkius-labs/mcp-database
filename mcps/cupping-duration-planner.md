# Cupping Duration Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cupping-duration-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Precision planning for cupping therapy sessions, determining suction, timing, and volume.

## Description
This MCP server provides a precision planning engine for cupping therapy. It calculates optimal suction levels, placement durations, and cup counts based on therapeutic protocols and client sensitivity. Practitioners can use `plan_session` to generate complete session plans, `get_area_sensitivity` to check anatomical constraints, `validate_protocol_safety` to ensure client safety, and `get_aftercare_recommendations` for post-treatment guidance.


## Available Tools (4)
- **get_aftercare_recommendations**: Provides specific post-treatment guidance based on the intensity of the session
- **get_area_sensitivity**: Inquires about the typical sensitivity levels and recommended suction constraints for a specific body part
- **plan_session**: Generates a complete cupping therapy session plan based on client and condition parameters
- **validate_protocol_safety**: Checks if the requested combination of parameters falls within safe therapeutic bounds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cupping Duration Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a static cupping session for muscle tension on the back for a client with medium tolerance."

**🤖 AI Agent:**
> The session plan for the back includes a medium suction level, 5 minutes per placement, and a total of 8 cups. Please follow the standard hydration aftercare.

---

**👤 You:**
> "How sensitive is the neck area for cupping?"

**🤖 AI Agent:**
> The neck is a small area with low tolerance. It is recommended to use low suction levels for this region.

---

**👤 You:**
> "Is it safe to use high suction for circulation on a client with low tolerance?"

**🤖 AI Agent:**
> No, that combination is unsafe. High-intensity suction paired with low client tolerance is flagged as a safety risk.


## ❓ FAQ

**Q: How does the planner determine suction levels?**
Suction levels are calculated by analyzing the intersection of the target therapeutic condition and the client's specific sensitivity level.

**Q: Can I check if a session is safe for a specific client?**
Yes, you can use the `validate_protocol_safety` tool to verify if the combination of cup type, condition, and client tolerance falls within safe therapeutic bounds.

**Q: Does it provide instructions for after the session?**
Yes, the `get_aftercare_recommendations` tool provides specific post-treatment guidance based on the intensity used during the session.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cupping-duration-planner](https://vinkius.com/en/ai-agent-connect/cupping-duration-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cupping Duration Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cupping-duration-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cupping Duration Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cupping-duration-planner": {
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
