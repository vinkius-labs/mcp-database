# Pet Enrichment Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pet-enrichment-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [pet-care](../categories/pet-care.md)

Generates personalized, weekly enrichment plans for pets by assessing breed needs and home environment constraints.

## Description
The pet's routine shouldn't be a guessing game. Boredom leads to destructive behavior; inconsistent care fails to meet true physical or cognitive needs. This planner solves that by creating structured, personalized weekly enrichment schedules.

### How it works (Mechanism)
This MCP acts as a bridge between raw pet data and actionable daily plans. It uses three core tools:

1.  **`get_pet_base_profile`**: Establishes the foundation by calculating the pet's baseline physical capabilities, trainability index, and suggested energy level based on its species, breed, and age.
2.  **`assess_environment_capacity`**: Models your living space (apartment or yard) to determine what activities are physically possible and safe within the home's constraints. This prevents recommending dangerous jumps in a confined area.
3.  **`generate_weekly_plan`**: The synthesis tool. It combines the pet profile and environment assessment to generate seven days of tailored plans, ensuring both physical exercise and mental stimulation (cognitive work) are scheduled daily. 

The output is a safe, comprehensive, and balanced schedule that respects all biological and structural limitations.

### Advantage
Instead of random play sessions, you receive a concrete plan detailing exactly what to do, when, and for how long. This ensures optimal physical fitness and sustained mental engagement for your companion.


## Available Tools (3)
- **assess_environment_capacity**: Returns max activity duration, restriction matrix, and activity type modifier.

Model the physical limitations and benefits of the pet's living environment
- **get_pet_base_profile**: Use this as the foundation for enrichment planning.

Retrieve a pet's baseline physical capabilities and behavioral tendencies
- **generate_weekly_plan**: Focus area can be Cognitive Focus, Joint Conditioning, or Balanced.

Generate a full structured weekly enrichment plan with physical and cognitive activities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Enrichment Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My dog is a 3-year-old Golden Retriever living in an apartment. I want the plan to focus on joint conditioning."

**🤖 AI Agent:**
> Based on your input, the system first runs `get_pet_base_profile` and then uses `assess_environment_capacity`. Finally, it calls `generate_weekly_plan(..., focusArea='Joint Conditioning')`, providing a 7-day schedule with low-impact indoor activities.

---

**👤 You:**
> "Generate an enrichment plan for my senior cat (12 years) in a house with a small yard. Balance is the focus."

**🤖 AI Agent:**
> The planner uses `get_pet_base_profile` to set low mobility expectations for the senior cat, then runs `assess_environment_capacity`. It concludes by calling `generate_weekly_plan(..., focusArea='Balanced')`, scheduling gentle outdoor sniffing and indoor puzzle time.

---

**👤 You:**
> "I have a puppy living in an apartment. I want the most physically demanding plan possible to build muscle."

**🤖 AI Agent:**
> The system will use `get_pet_base_profile` (which correctly sets high energy for a puppy) and `assess_environment_capacity`. The final plan from `generate_weekly_plan` will recommend structured indoor play, respecting the apartment's limitations.


## ❓ FAQ

**Q: Does this system account for different living spaces?**
Absolutely. The `assess_environment_capacity` tool analyzes your space--whether it's an apartment or a yard--to set hard limits on activity duration and type, ensuring all recommendations are safe for your specific home environment.

**Q: How does it handle age-related changes in needs?**
The `get_pet_base_profile` tool incorporates developmental science. It automatically adjusts the pet's suggested energy level and mobility rating based on age (e.g., senior pets receive lower-impact recommendations), ensuring activities are always appropriate.

**Q: What if I only want to focus on mental stimulation?**
You can specify a 'Cognitive Focus' in the final planning step. The `generate_weekly_plan` tool will then prioritize puzzle feeders, scent work, and training games while still ensuring minimal physical activity is included.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pet-enrichment-planner](https://vinkius.com/mcp/pet-enrichment-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Enrichment Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-enrichment-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Enrichment Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-enrichment-planner": {
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
