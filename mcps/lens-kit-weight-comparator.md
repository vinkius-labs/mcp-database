# Lens Kit Weight Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/lens-kit-weight-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utility](../categories/utility.md)

Evaluate camera kits based on weight, focal range, and user ergonomics.

## Description
This MCP server helps photographers select the most ergonomic camera setups. It analyzes kit mass against user weight and bag limits, evaluates focal range versatility, and ranks compatible kits. Use `rank_compatible_kits` to find the best setups for your needs, `compare_kit_weights` to check specific kit mass, `get_kit_optical_specs` for lens capabilities, and `evaluate_user_ergonomics` to ensure your gear is comfortable for your body weight.


## Available Tools (4)
- **compare_kit_weights**: Determines if a specific kit meets the user's weight constraints and calculates its total mass
- **get_kit_optical_specs**: Evaluates the versatility of a kit by checking its focal length capabilities
- **evaluate_user_ergonomics**: Suggests whether a kit is physically suitable for a user based on their body mass and the kit's weight
- **rank_compatible_kits**: Provides a prioritized list of kits that satisfy a user's specific physical and optical requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lens Kit Weight Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find me the best camera kits for a 70kg user with a 5kg bag limit."

**🤖 AI Agent:**
> The best kits for you are the Travel/Compact Kit (3.2kg) and the Enthusiast Kit (4.5kg).

---

**👤 You:**
> "What is the focal range of kit 'pro-setup-01'?"

**🤖 AI Agent:**
> The kit 'pro-setup-01' has a focal range of 24mm to 200mm with 3 lenses.

---

**👤 You:**
> "Is a 6kg kit ergonomic for someone weighing 60kg?"

**🤖 AI Agent:**
> The suitability score is low because the kit weight is 10% of your body weight.


## ❓ FAQ

**Q: How does the tool calculate kit weight?**
The total weight is calculated by summing the mass of the camera body, all selected lenses, and essential accessories.

**Q: Can I filter kits by focal length?**
Yes, you can use `rank_compatible_kits` to provide minimum and maximum focal length requirements to find the best matches.

**Q: What is ergonomic suitability?**
It is a score that compares the kit's weight to your own body mass to ensure your gear is comfortable to carry.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/lens-kit-weight-comparator](https://vinkius.com/en/ai-agent-connect/lens-kit-weight-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lens Kit Weight Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lens-kit-weight-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lens Kit Weight Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lens-kit-weight-comparator": {
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
