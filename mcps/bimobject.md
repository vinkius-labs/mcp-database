# BIMobject MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bimobject)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bimobject-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bimobject-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Access BIMobject marketplace — search building products, download technical files, and manage manufacturer data directly from any AI agent.

## Description
Connect your AI agents to **BIMobject**, the world's leading BIM content platform. This MCP provides 10 tools to search the marketplace, retrieve detailed product specifications, and access BIM files for AEC (Architecture, Engineering, and Construction) workflows.

### What you can do

- **Product Discovery** — Search for specific building products and materials using keywords and filters
- **Technical Specs** — Retrieve granular metadata and manufacturer details for BIM objects
- **File Access** — List available BIM formats (Revit, ArchiCAD, IFC, etc.) for any product
- **Brand Analysis** — Explore manufacturer profiles and their full digital product catalogs

### How it works

1. Subscribe to this server
2. Sign up at the [**BIMobject Developer Portal**](https://developer.bimobject.com/)
3. Register your application to obtain your **API Key** (Access Token)
4. Connect your account to Vurb to start automating your AEC content orchestration.

### Who is this for?

- **Architects & Engineers** — quickly find and specify real-world building products in their designs
- **BIM Managers** — automate the retrieval of object metadata and file updates
- **AEC Software Developers** — integrate BIM content discovery into custom construction applications


## Available Tools
- **get_brand_details**: Get details for a specific brand
- **get_me**: Get current user profile
- **get_product_files**: List files available for a product
- **get_product_details**: Get detailed information for a specific product
- **list_brands**: List manufacturers and brands
- **list_categories**: List product categories
- **list_classifications**: List classification systems
- **list_featured_products**: List featured marketplace products
- **list_latest_products**: List latest added products
- **search_products**: Search for BIM products in the marketplace


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BIMobject** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search BIMobject for 'sustainable insulation' and list the first 5 results."

**🤖 AI Agent:**
> I've searched the BIMobject marketplace. Here are the top 5 results for 'sustainable insulation': 1. EcoWool Batt (ID: pr_1), 2. BioBoard Rigid (ID: pr_2)... Would you like the technical specs for any of these?

---

**👤 You:**
> "Get all available Revit files for product ID 'p_999'."

**🤖 AI Agent:**
> Retrieving file list for product 'Modern Windows' (ID: p_999)... I've found 2 Revit files: 1. Fixed Frame (v2023), 2. Sliding Unit (v2023). Both are available for immediate download.

---

**👤 You:**
> "List all brands configured in my BIMobject project."

**🤖 AI Agent:**
> Fetching manufacturers... I found several brands associated with your profile, including Rockfon, Knauf, and Armstrong Ceiling Solutions. Which one would you like to explore?


## Installation & Usage

To install and use the **BIMobject** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bimobject](https://vinkius.com/mcp/bimobject)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
