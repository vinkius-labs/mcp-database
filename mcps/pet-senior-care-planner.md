# Pet Senior Care Planner MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pet-senior-care-planner)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pet-senior-care-planner-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pet-senior-care-planner-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Identify pet life stages and generate customized veterinary and lifestyle protocols.

## Description
The Pet Senior Care Planner helps owners manage the aging process of their pets. By using `identify_pet_life_stage`, you can determine if a pet is in the Adult, Senior, or Geriatric phase based on species, breed, and age. Once the stage is identified, use `get_veterinary_protocol` to find recommended checkup frequencies and diagnostic tests, and `get_lifestyle_recommendations` to discover necessary dietary and exercise adjustments for optimal health during aging.


## Available Tools
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


## Installation & Usage

To install and use the **Pet Senior Care Planner** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pet-senior-care-planner](https://vinkius.com/mcp/pet-senior-care-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
