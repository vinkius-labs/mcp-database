# Muscle Knot Mapping MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/muscle-knot-mapping)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Maps muscle knots to clinical referral patterns and treatment priorities.

## Description
This MCP server provides diagnostic support for identifying myofascial trigger points. It connects AI agents to clinical mapping data to determine the likely muscle source of pain, describe characteristic pain patterns, evaluate treatment urgency, and identify functionally linked muscles. Use `identify_trigger_source` to find the muscle responsible for referred pain, `get_pain_pattern` to understand how pain radiates, `analyze_knot_severity` to determine treatment priority, and `map_muscle_relationships` to find related muscle groups.


## Available Tools (4)
- **get_pain_pattern**: Describes the full extent and direction of pain associated with a specific muscle knot
- **analyze_knot_severity**: Evaluates how urgently a knot needs treatment based on its physical attributes
- **identify_trigger_source**: Determines the most likely muscle containing the trigger point based on the location of the perceived pain
- **map_muscle_relationships**: Identifies neighboring or functionally linked muscles that might be contributing to the pain


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Muscle Knot Mapping** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have pain in my temple, but it feels like it's coming from my neck. Is this referred pain?"

**🤖 AI Agent:**
> The pain in your temple is likely referred pain originating from a trigger point in your upper trapezius muscle.

---

**👤 You:**
> "How severe is a deep knot in my shoulder that makes it hard to lift my arm?"

**🤖 AI Agent:**
> A deep knot with severe functional impact is classified as a high priority for treatment.

---

**👤 You:**
> "What is the typical pain pattern for the levator scapulae muscle?"

**🤖 AI Agent:**
> The levator scapulae typically causes pain that radiates toward the angle of the neck and the top of the shoulder blade.


## ❓ FAQ

**Q: How does this tool help identify the source of pain?**
By using the `identify_trigger_source` tool, the agent can analyze whether pain is local or referred to find the specific muscle containing the knot.

**Q: Can I determine how urgent a muscle knot is?**
Yes, the `analyze_knot_severity` tool evaluates depth, tenderness, and functional impact to assign a treatment priority level.

**Q: Does it identify related muscles?**
Yes, the `map_muscle_relationships` tool identifies neighboring or functionally linked muscles that share innervation or functional groups.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/muscle-knot-mapping](https://vinkius.com/en/ai-agent-connect/muscle-knot-mapping)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Muscle Knot Mapping** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `muscle-knot-mapping` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Muscle Knot Mapping** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "muscle-knot-mapping": {
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
