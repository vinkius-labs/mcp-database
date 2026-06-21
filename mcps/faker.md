# Faker MCP Server

Generate high-quality mock data for development and testing — including addresses, persons, companies, and products in multiple locales.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/faker)

## Overview
**Category:** developer-tools
**Tools Count:** 11

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


## Installation & Usage

To install and use the **Faker** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/faker](https://vinkius.com/mcp/faker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
