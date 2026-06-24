# Pet Age Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pet-age-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate human-equivalent ages for dogs and cats using species-specific biological growth curves.

## Description
The Pet Age Converter is a precision biological aging engine that moves beyond the simplistic 'one year equals seven years' myth. By utilizing non-linear, species-specific growth curves, this MCP server provides accurate human-age equivalents for pets. For dogs, the tool accounts for size-dependent aging trajectories, applying different models for small, medium, and large breeds. For cats, it implements a unified feline maturation curve. Use `convert_dog_age` to find the human age of a dog based on its breed size, `convert_cat_age` for cats, and `get_pet_life_stage` to identify biological milestones like Puppy, Adult, or Senior.


## Available Tools (3)
- **convert_cat_age**: Convert cat age to human equivalent age
- **convert_dog_age**: Convert dog age to human equivalent age
- **get_pet_life_stage**: Get the life stage of a pet


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Age Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How old is a 3-year-old small dog in human years?"

**🤖 AI Agent:**
> A 3-year-old small dog is approximately 28 years old in human years.

---

**👤 You:**
> "What is the human age of a 5-year-old cat?"

**🤖 AI Agent:**
> A 5-year-old cat is approximately 36 years old in human years.

---

**👤 You:**
> "Is a 10-year-old large dog considered a senior?"

**🤖 AI Agent:**
> Yes, a 10-year-old large dog is in the Senior life stage.


## ❓ FAQ

**Q: Why not just multiply the pet's age by 7?**
The '7-year rule' is biologically inaccurate. Pets undergo rapid development in their early years and a different maturation process as they age. Our tools, such as `convert_dog_age`, use scientifically backed non-linear curves to provide much more precise estimates.

**Q: How does dog size affect the calculation?**
Canine aging is heavily influenced by breed mass. Small dogs, medium dogs, and large dogs follow distinct biological trajectories. The `convert_dog_age` tool requires a size category to apply the correct growth model.

**Q: Can I determine if my pet is a senior?**
Yes. After calculating the human-equivalent age, you can use the `get_pet_life_stage` tool to determine if your pet is in the Infant, Adult, Senior, or Geriatric stage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pet-age-converter](https://vinkius.com/mcp/pet-age-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Age Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-age-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Age Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-age-converter": {
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
