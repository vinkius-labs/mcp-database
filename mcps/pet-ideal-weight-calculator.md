# Pet Ideal Weight Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pet-ideal-weight-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Determine and classify your pet's weight status based on species, breed, and sex.

## Description
The Pet Ideal Weight Calculator helps pet owners monitor their animal's health by comparing current weight against biological ideal ranges. Using the `analyze_pet_health` tool, you can identify if a pet is Underweight, Ideal, or Overweight. The system uses specific data for species like Dog and Cat to provide precise recommendations based on breed and sex.


## Available Tools (3)
- **get_breed_catalog**: Get breeds and weight ranges for a species
- **list_supported_species**: g., Dog, Cat).

List all supported animal species
- **analyze_pet_health**: Analyze a pet's weight status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Ideal Weight Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is my Golden Retriever male weighing 35kg overweight?"

**🤖 AI Agent:**
> A 35kg male Golden Retriever is classified as Overweight. The ideal weight range for this breed and sex is 29kg - 34kg.

---

**👤 You:**
> "What is the ideal weight for a female Siamese cat weighing 3kg?"

**🤖 AI Agent:**
> A 3kg female Siamese cat is classified as Underweight. The target range is 3.5kg - 4.5kg.

---

**👤 You:**
> "Check the health status of a 20kg male Bulldog."

**🤖 AI Agent:**
> A 20kg male Bulldog is classified as Underweight. The ideal range for this breed and sex is 23kg - 28kg.


## ❓ FAQ

**Q: How do I check my pet's weight status?**
You can use the `analyze_pet_health` tool by providing the species, breed, sex, and current weight of your pet.

**Q: What species are supported?**
You can use the `list_supported_species` tool to see a complete list of all animals currently in our database.

**Q: How do I find the correct breed name?**
Use the `get_breed_catalog` tool with a specific species name to retrieve all available breeds and their weight ranges.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pet-ideal-weight-calculator](https://vinkius.com/mcp/pet-ideal-weight-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Ideal Weight Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-ideal-weight-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Ideal Weight Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-ideal-weight-calculator": {
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
