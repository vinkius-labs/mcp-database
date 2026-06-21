# Faker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/faker)
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


## Available Tools (11)
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


## ❓ FAQ

**Q: Can I generate data in specific languages like Brazilian Portuguese or French?**
Yes! Use the `_locale` parameter with codes like `pt_BR` or `fr_FR`. This ensures that names, addresses, and other fields follow the conventions of that specific region.

**Q: How do I ensure I get the same random data every time for my tests?**
You can use the `_seed` parameter. By providing the same integer seed in your request, the generator will produce identical results, which is perfect for regression testing.

**Q: What is the maximum amount of data I can request in a single call?**
The `_quantity` parameter allows you to request between 1 and 1000 rows of data per tool execution.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/faker](https://vinkius.com/mcp/faker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Faker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `faker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Faker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "faker": {
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
