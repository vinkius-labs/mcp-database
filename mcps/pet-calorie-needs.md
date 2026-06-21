# Pet Calorie Needs MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pet-calorie-needs)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [nutrition](../categories/nutrition.md)

Calculate precise daily energy requirements (RER and MER) for pets based on weight and lifestyle.

## Description
This MCP server provides veterinary-standard calculations for a pet's nutritional needs. Using the `calculate_rer` tool, you can determine the Resting Energy Requirement based on metabolic weight. By applying lifestyle multipliers via `calculate_mer`, you can find the Maintenance Energy Requirement (MER) for various states like neutered, intact, or athletic. Use `list_lifestyle_factors` to see all available activity and physiological multipliers.


## Available Tools
- **calculate_mer**: Calculate the Maintenance Energy Requirement (MER) for a pet
- **calculate_rer**: 75 to find the baseline calories needed at rest.

Calculate the Resting Energy Requirement (RER) for a pet
- **list_lifestyle_factors**: List all available lifestyle factors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Calorie Needs** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many calories does a 10kg dog need if it is neutered?"

**🤖 AI Agent:**
> A 10kg neutered dog has an RER of approximately 501 kcal and a daily maintenance requirement (MER) of about 626 kcal.

---

**👤 You:**
> "Calculate the RER for a 5kg cat."

**🤖 AI Agent:**
> The Resting Energy Requirement (RER) for a 5kg cat is approximately 297 kcal.

---

**👤 You:**
> "What are the available lifestyle factors?"

**🤖 AI Agent:**
> The available lifestyle factors include neutered, intact, pregnant, lactating, athletic, and weight loss.


## ❓ FAQ

**Q: What is RER?**
Resting Energy Requirement (RER) is the minimum amount of energy needed to maintain vital functions while the animal is at rest.

**Q: How do I know which lifestyle factor to use?**
You can use the `list_lifestyle_factors` tool to see a complete list of available keys like 'neutered' or 'athletic'.

**Q: Does this account for different breeds?**
The calculation is based on metabolic weight (kg^0.75), which is a standard veterinary approach that inherently accounts for scaling across different sizes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pet-calorie-needs](https://vinkius.com/mcp/pet-calorie-needs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Calorie Needs** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pet-calorie-needs` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Calorie Needs** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-calorie-needs": {
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
