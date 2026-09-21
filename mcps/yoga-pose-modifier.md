# Yoga Pose Modifier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/yoga-pose-modifier)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Intelligent yoga pose adaptations based on physical limitations and available props.

## Description
This MCP server provides intelligent yoga pose adaptations to ensure safe and accessible practice. By connecting your AI agent to specialized yoga modification principles, you can receive specific guidance on `get_pose_modifications` to adapt poses for mobility issues or strength deficits. Use `get_prop_guidance` to learn how to position blocks or straps, `get_alignment_refinement` for precise injury-prevention cues, and `get_progression_pathway` to build a step-by-step journey toward full pose expression.


## Available Tools (4)
- **get_alignment_refinement**: Provide high-precision alignment instructions to prevent injury during a modified pose
- **get_pose_modifications**: Find specific ways to adapt a standard yoga pose based on a user's profile
- **get_progression_pathway**: Outline a step-by-step journey from a highly modified version of a pose toward the full expression
- **get_prop_guidance**: Determine exactly how to position and utilize specific yoga props for a given pose and limitation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Yoga Pose Modifier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have lower back tension and want to do Plank. What are my options?"

**🤖 AI Agent:**
> For lower back tension in Plank, you can try a modified version using blocks under your hands or performing the pose on your knees to reduce spinal load.

---

**👤 You:**
> "How should I use a strap for Tree Pose if I have limited hip mobility?"

**🤖 AI Agent:**
> You can loop the strap around your ankle to provide stability and bring your foot closer to your inner thigh without overstretching.

---

**👤 You:**
> "Give me alignment cues for a modified Warrior II for a beginner with knee sensitivity."

**🤖 AI Agent:**
> Keep your front knee aligned directly over your ankle and avoid letting it collapse inward to protect the joint.


## ❓ FAQ

**Q: How can I adapt a pose for wrist pain?**
You can use `get_pose_modifications` by specifying 'wrist mobility' as your limitation type to find suitable adaptations.

**Q: Can I learn how to use yoga blocks with this tool?**
Yes, use `get_prop_guidance` and list 'block' in your available props to receive specific setup instructions.

**Q: How do I progress from a modified pose to a standard one?**
The `get_progression_pathway` tool provides a logical, incremental sequence of stages to help you move toward the full expression of a pose.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/yoga-pose-modifier](https://vinkius.com/en/ai-agent-connect/yoga-pose-modifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Yoga Pose Modifier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `yoga-pose-modifier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Yoga Pose Modifier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "yoga-pose-modifier": {
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
