# Faker MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/faker)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/faker-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/faker-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Generate high-quality mock data for development and testing — including addresses, persons, companies, and products in multiple locales.

## Description
Connect the **Faker** MCP server to your AI agent to instantly generate realistic placeholder data for your applications. Whether you need to populate a database, test an API, or create UI mockups, Faker provides a comprehensive suite of tools to generate structured data on demand.

### What you can do

- **Personal & User Data** — Generate mock profiles, names, and user credentials with `get_persons` and `get_users`.
- **Business Entities** — Create fake companies, VAT numbers, and products using `get_companies` and `get_products`.
- **Localization** — Support for over 70 locales to ensure your data looks authentic for any region using the `_locale` parameter.
- **Media & Content** — Fetch placeholder images and random text blocks for UI design via `get_images` and `get_texts`.
- **Financial Data** — Generate safe credit card information for checkout flow testing with `get_credit_cards`.

### How it works

1. Subscribe to this server
2. Enter your FakerAPI credentials if required
3. Start generating structured data directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — quickly seed databases or mock API responses without manual entry.
- **QA Engineers** — create diverse test cases with randomized but structured data.
- **Product Designers** — fill prototypes with realistic content instead of 'lorem ipsum'.


## Available Tools
- **get_addresses**: Can be filtered by country_code.

Generate mock address data
- **get_books**: Generate mock book information
- **get_companies**: Generate mock company data
- **get_credit_cards**: Generate mock credit card information
- **get_custom**: Pass a JSON object mapping field names to Faker types (e.g. {"myField": "name", "otherField": "email"}).

Generate custom mock data structures
- **get_images**: Supports sources like Picsum and types like "any" or "pokemon".

Generate mock image URLs
- **get_persons**: Supports genders "male", "female", and "other".

Generate mock personal information
- **get_places**: Generate mock place data
- **get_products**: Generate mock product data
- **get_texts**: Generate mock text content
- **get_users**: Generate mock user account data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Faker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate 5 fake company profiles with websites and VAT numbers."

**🤖 AI Agent:**
> I've generated 5 mock companies for you, including 'TechFlow Solutions' and 'Global Logistics Inc.', complete with their registered VAT numbers and official websites.

---

**👤 You:**
> "I need 10 random addresses in Germany using the de_DE locale."

**🤖 AI Agent:**
> Here are 10 German addresses. They include street names like 'Hauptstraße' and 'Goethestraße' with valid postal codes and city names formatted for the de_DE region.

---

**👤 You:**
> "Give me 3 mock books with titles and authors."

**🤖 AI Agent:**
> I've retrieved 3 mock books: 'The Silent Echo' by Jane Doe, 'Digital Horizons' by John Smith, and 'Beyond the Veil' by Alice Johnson.


## Installation & Usage

To install and use the **Faker** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/faker](https://vinkius.com/mcp/faker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
