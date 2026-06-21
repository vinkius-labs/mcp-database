# Faker Data Generator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/faker-data-generator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/faker-data-generator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/faker-data-generator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Generate realistic fake data in seconds — names, emails, addresses, credit cards, companies, and more. 60+ locales including Brazilian Portuguese. The most complete data generator in the ecosystem, with 5M+ weekly downloads.

## Description
Your agent is building a demo environment. It needs 50 user profiles with realistic names, valid-looking emails, and Brazilian addresses. If you let the AI generate them, you'll get 50 variations of 'John Doe' with emails at 'example.com'.

This MCP uses @faker-js/faker (5M+ weekly downloads) to generate contextually rich, locale-aware test data across 10 categories. Brazilian names for pt_BR, Japanese addresses for ja, German companies for de.

### The Superpowers

- **10 Categories:** person, internet, company, address, finance, commerce, lorem, date, image, phone.
- **60+ Locales:** Real Brazilian CPF-style names, Japanese kanji, French addresses — not just English translated.
- **Batch Generation:** Up to 50 records per request for database seeding.
- **Cryptographic Quality:** Uses secure randomness — each call produces unique, non-repeating data.


## Available Tools
- **generate_fake_data**: Categories: person, internet, company, address, finance, commerce, lorem, date, image, phone. Each category returns multiple related fields. Set count (max 50) for batch generation. Locale changes names/addresses to match the target country (e.g. "pt_BR" for Brazilian names).

Generates realistic fake data: names, emails, addresses, companies, products, finances, lorem ipsum, dates, and more. Supports 60+ locales


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Faker Data Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate 10 realistic user profiles with Brazilian names for our demo environment."

**🤖 AI Agent:**
> 10 profiles with Brazilian names, emails, and job titles generated in pt_BR locale.

---

**👤 You:**
> "Create fake credit card numbers and IBANs for testing our payment flow."

**🤖 AI Agent:**
> Finance data: valid-format credit card numbers, IBANs, BICs, and transaction amounts.

---

**👤 You:**
> "Seed our staging database with 50 company records including addresses."

**🤖 AI Agent:**
> 50 company records with names, catch phrases, and full address details.


## Installation & Usage

To install and use the **Faker Data Generator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/faker-data-generator](https://vinkius.com/mcp/faker-data-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
