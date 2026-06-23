# Pet Senior Care Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pet-senior-care-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Identify pet life stages and generate customized veterinary and lifestyle protocols.

## Description
The Pet Senior Care Planner helps owners manage the aging process of their pets. By using `identify_pet_life_stage`, you can determine if a pet is in the Adult, Senior, or Geriatric phase based on species, breed, and age. Once the stage is identified, use `get_veterinary_protocol` to find recommended checkup frequencies and diagnostic tests, and `get_lifestyle_recommendations` to discover necessary dietary and exercise adjustments for optimal health during aging.


## Available Tools (3)
- **get_lifestyle_recommendations**: Provides lifestyle recommendations based on life stage
- **get_veterinary_protocol**: Provides veterinary monitoring requirements for a life stage
- **identify_pet_life_stage**: Determines the current biological life stage of a pet


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Senior Care Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My 8-year-old Golden Retriever is a dog. What is his life stage?"

**🤖 AI Agent:**
> Based on the `identify_pet_life_stage` tool, an 8-year-old Golden Retriever is classified as being in the Senior or Geriatric stage due to the large breed aging scale.

---

**👤 You:**
> "What veterinary tests are needed for a geriatric cat?"

**🤖 AI Agent:**
> By calling `get_veterinary_protocol` for a cat in the Geriatric stage, you will find recommendations for increased visit frequency and tests like Blood Chemistry and Dental X-rays.

---

**👤 You:**
> "Give me lifestyle tips for a senior dog."

**🤖 AI Agent:**
> Using `get_lifestyle_recommendations`, the tool suggests dietary adjustments like calorie control and exercise modifications such as low-impact activities to protect joint health.


## ❓ FAQ

**Q: How does the tool determine a pet's life stage?**
The `identify_pet_life_stage` tool evaluates the species, breed size, and chronological age to identify if the pet is Adult, Senior, or Geriatric.

**Q: What kind of medical information can I get?**
Using `get_veterinary_protocol`, you can retrieve the recommended frequency for veterinary visits and a list of essential diagnostic tests for the pet's specific life stage.

**Q: Does it provide diet and exercise advice?**
Yes, the `get_lifestyle_recommendations` tool provides specific dietary adjustments and physical activity modifications to support your pet's health as they age.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pet-senior-care-planner](https://vinkius.com/mcp/pet-senior-care-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Senior Care Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-senior-care-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Senior Care Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-senior-care-planner": {
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
