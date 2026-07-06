# Pet Food Portion Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pet-food-portion-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate precise daily food portions for dogs and cats based on weight, activity, and life stage.

## Description
This MCP server provides a scientific approach to pet nutrition by calculating the exact daily kilocalorie requirements and physical food volumes needed for your pets. Using the Resting Energy Requirement (RER) formula, it adjusts for species (dog or cat), body condition, activity level, life stage, and neutering status. The tool also converts these calorie needs into measurable portions like cups or cans based on the specific caloric density of your pet's food. With tools like `calculate_kcal_requirement`, `calculate_food_portion`, and `verify_pet_profile`, you can ensure your pet is receiving the optimal amount of nutrition for their unique lifestyle.


## Available Tools (3)
- **calculate_food_portion**: Calculate the physical volume of food to feed
- **calculate_kcal_requirement**: Calculate daily kilocalorie requirement for a pet
- **verify_pet_profile**: Verify if a pet profile is biologically plausible


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Food Portion Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many calories does my 10kg adult dog need if he is very active and neutered?"

**🤖 AI Agent:**
> An active, neutered 10kg adult dog requires approximately 456 kcal per day.

---

**👤 You:**
> "If my cat needs 250 kcal/day and my food is 350 kcal/cup, how much should I feed?"

**🤖 AI Agent:**
> You should feed approximately 0.71 cups of food per day.

---

**👤 You:**
> "Is a 50kg kitten profile realistic?"

**🤖 AI Agent:**
> No, a 50kg weight for a kitten is not biologically plausible.


## ❓ FAQ

**Q: How accurate are the calorie calculations?**
The calculations use the standard Resting Energy Requirement (RER) formula, adjusted by scientifically recognized multipliers for activity level, life stage, and neutering status.

**Q: Which pet species are supported?**
Currently, the calculator supports both dogs and cats.

**Q: Can I use this for different food brands?**
Yes. By providing the caloric density (kcal per cup or can) of your specific brand, the `calculate_food_portion` tool will give you an accurate volume measurement.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pet-food-portion-calculator](https://vinkius.com/mcp/pet-food-portion-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Food Portion Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-food-portion-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Food Portion Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-food-portion-calculator": {
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
