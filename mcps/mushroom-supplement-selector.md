# Mushroom Supplement Selector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/mushroom-supplement-selector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Personalized functional mushroom recommendations based on health goals.

## Description
This MCP server provides expert-level guidance on functional mushroom supplementation. By analyzing your specific health objectives--such as immunity, cognition, energy, or stress management--it identifies the most effective mushrooms for your needs. Use `query_mushroom_recommendations` to find the right mushrooms, `check_stack_compatibility` to ensure your combinations are synergistic rather than redundant, and `calculate_dosing_schedule` to receive precise timing and dosage instructions. You can also use `search_mushroom_properties` to dive deep into the bioactive compounds and benefits of specific species.


## Available Tools (4)
- **check_stack_compatibility**: Validates if a specific combination of mushrooms is safe or synergistic
- **calculate_dosing_schedule**: Provides specific instructions on when and how much to take based on the selected mushrooms
- **query_mushroom_recommendations**: Generates a personalized recommendation of mushrooms based on the user's profile
- **search_mushroom_properties**: Retrieves detailed biological properties of a single mushroom


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mushroom Supplement Selector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to improve my focus and energy. I currently take Vitamin D. I prefer capsules."

**🤖 AI Agent:**
> Based on your goals, I recommend Lion's Mane for cognition and Cordyceps for energy. You should take 500mg of Lion's Mane in the morning and 1000mg of Cordyceps before your workout.

---

**👤 You:**
> "Is it good to take Reishi and Chaga together?"

**🤖 AI Agent:**
> Yes, Reishi and Chaga are synergistic for immune support and stress management.

---

**👤 You:**
> "Tell me about the benefits of Lion's Mane."

**🤖 AI Agent:**
> Lion's Mane is known for supporting cognitive function, memory, and nerve health through active compounds like erinacines.


## ❓ FAQ

**Q: How do I get a recommendation?**
Provide your health goals, current supplements, and preferred form to the `query_mushroom_recommendations` tool to receive a personalized list.

**Q: Can I check if my mushroom stack is safe?**
Yes, use the `check_stack_compatibility` tool to determine if your chosen mushrooms are synergistic or redundant.

**Q: Will I know when to take my supplements?**
Yes, the `calculate_dosing_schedule` tool provides specific timing and dosage instructions for your selected mushrooms.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/mushroom-supplement-selector](https://vinkius.com/en/ai-agent-connect/mushroom-supplement-selector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mushroom Supplement Selector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mushroom-supplement-selector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mushroom Supplement Selector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mushroom-supplement-selector": {
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
