# Crystal Matcher MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crystal-matcher)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/crystal-matcher-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/crystal-matcher-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [wellness](../categories/wellness.md)

Connect AI agents to a curated catalog of crystals based on intent, element, and chakra.

## Description
## Connect AI Agents to the Crystal Matcher Catalog

Finding the right crystal for a specific intention can be complex. Whether you are seeking protection, love, abundance, or healing, matching your energetic needs with the correct stone requires knowledge of properties, elements, and chakras.

This MCP server gives AI agents direct access to an extensive catalog of over 80 crystals through tools like `query_crystals_by_intent`, `get_crystal_details`, `filter_crystals_by_element`, and `find_crystals_by_chakra`. Agents can interpret a user's spiritual or emotional goal and return precise recommendations based on vibrational matching.

Instead of manual searching, ask your AI assistant: *"Which crystals are good for the Heart chakra?"* The agent calls `find_crystals_by_chakra`, retrieves the list, and presents the associated stones and their properties.

Connects through Vinkius Edge -- one URL, one token, no API keys to manage.


## Available Tools
- **get_crystal_details**: Get detailed information about a specific crystal
- **filter_crystals_by_element**: Filter crystals by their associated element
- **find_crystals_by_chakra**: Find crystals associated with a specific chakra
- **query_crystals_by_intent**: Find crystals based on a spiritual or emotional intent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crystal Matcher** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am feeling very anxious and need grounding. Which crystals should I use?"

**🤖 AI Agent:**
> To help with grounding and anxiety, I recommend looking into stones associated with the Earth element or the Root chakra. Based on your need for grounding, you might consider using Black Tourmaline or Hematite, which are known for their stabilizing properties.

---

**👤 You:**
> "List all crystals associated with the Heart chakra."

**🤖 AI Agent:**
> I found several crystals for the Heart chakra, including Rose Quartz, Jade, and Emerald. These stones are primarily used to promote love, compassion, and emotional healing.

---

**👤 You:**
> "Tell me more about the properties of Amethyst."

**🤖 AI Agent:**
> **Amethyst**

- **Properties**: Calm, Clarity, Protection
- **Element**: Air
- **Chakra**: Third Eye

Amethyst is a powerful stone for spiritual protection and enhancing intuition.


## Installation & Usage

To install and use the **Crystal Matcher** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crystal-matcher](https://vinkius.com/mcp/crystal-matcher)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
