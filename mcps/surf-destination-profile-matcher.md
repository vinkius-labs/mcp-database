# Surf Destination Profile Matcher MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/surf-destination-profile-matcher)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Find your perfect surf spot using deterministic profile matching.

## Description
This MCP server connects AI agents to a deterministic matching engine that identifies the best surf destinations based on a surfer's specific profile. By analyzing skill level, wave type preference, and crowd tolerance, the engine calculates a precise match score for various global locations. Use `find_best_destinations` to get a ranked list of top spots, `get_destination_details` to inspect specific location characteristics, or `validate_surfer_profile` to ensure your preferences align with the engine's supported parameters.


## Available Tools (3)
- **find_best_destinations**: Identifies the most compatible surf destinations for a specific surfer profile
- **get_destination_details**: Retrieves the specific characteristics of a single surf destination
- **validate_surfer_profile**: Checks if a set of surfer preferences is valid according to the engine's constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surf Destination Profile Matcher** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the best surf destinations for an advanced surfer who prefers reef breaks and can handle high crowds."

**🤖 AI Agent:**
> The best destination for you is Bali_Uluwatu with a match score of 100.

---

**👤 You:**
> "What are the details for the Bali_Uluwatu destination?"

**🤖 AI Agent:**
> Bali_Uluwatu is a reef break destination designed for advanced surfers with high crowd levels.

---

**👤 You:**
> "Is 'pro' a valid skill level for the surf matcher?"

**🤖 AI Agent:**
> No, 'pro' is not a valid skill level. Supported levels are beginner, intermediate, and advanced.


## ❓ FAQ

**Q: How are the surf destinations matched?**
The engine uses a mathematical distance calculation between your provided attributes (skill, wave type, and crowd tolerance) and fixed destination profiles to generate a match score from 0 to 100.

**Q: What skill levels are supported?**
The engine supports three skill levels: beginner, intermediate, and advanced.

**Q: Can I check if my preferences are valid?**
Yes, you can use the `validate_surfer_profile` tool to verify that your skill level, wave type, and crowd tolerance inputs are within the allowed domain values.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/surf-destination-profile-matcher](https://vinkius.com/ai-agent-connect/surf-destination-profile-matcher)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surf Destination Profile Matcher** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surf-destination-profile-matcher` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surf Destination Profile Matcher** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surf-destination-profile-matcher": {
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
