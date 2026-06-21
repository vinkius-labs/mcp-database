# Cannlytics Strain API MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cannlytics-strain-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cannlytics-strain-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cannlytics-strain-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Access cannabis strain data, effects, flavors, and similar strains via Cannlytics.

## Description
Connect **Cannlytics** to any AI agent and access structured, open cannabis strain data -- search strains, view effects and flavors, and discover similar strains through natural conversation.

### What you can do
- **Strain Search** -- Find cannabis strains by name or keyword
- **Effects & Flavors** -- Retrieve detailed positive, negative, and medical effects plus flavor profiles
- **Similar Strains** -- Discover related strains based on genetics or characteristics

### How it works
1. Subscribe to this server
2. Enter your Cannlytics API Key
3. Start exploring cannabis data from Claude, Cursor, or any MCP-compatible client

Cannlytics provides an open API for transparent cannabis data, serving consumers, researchers, and industry professionals.

### Who is this for?
- **Consumers** -- Verify strain effects and flavors before making a purchase
- **Budtenders** -- Quickly find similar strains and medical benefits to guide customers
- **Researchers** -- Access structured cannabis data for studies and market analysis


## Available Tools
- **get_effects**: Get reported effects for a specific strain
- **get_flavors**: g., earthy, sweet, citrus) for the strain.

Get flavor profile for a specific strain
- **get_strain**: Get detailed information for a specific cannabis strain
- **search_strains**: Use this to discover available strains in the Cannlytics database.

Search for cannabis strains by name or keyword
- **get_similar_strains**: Find strains similar to a specific strain


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cannlytics Strain API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for strains with 'Blue' in the name."

**🤖 AI Agent:**
> Found 5 strains: 1. Blue Dream. 2. Blueberry. 3. Blue Cheese. 4. Blue Cookies.

---

**👤 You:**
> "What are the effects of Sour Diesel?"

**🤖 AI Agent:**
> Effects: Energetic, Uplifted, Creative (Positive). Dry Mouth, Anxious (Negative). Stress, Pain (Medical).

---

**👤 You:**
> "Show me strains similar to OG Kush."

**🤖 AI Agent:**
> Similar strains: 1. Skywalker OG. 2. Bubba Kush. 3. Master Kush.


## Installation & Usage

To install and use the **Cannlytics Strain API** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cannlytics-strain-api](https://vinkius.com/mcp/cannlytics-strain-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
