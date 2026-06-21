# RandomUser API MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/randomuser-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/randomuser-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/randomuser-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate random user data — audit personas and locations via AI.

## Description
Empower your AI agent to orchestrate your entire persona research and data synthesis workflow with **RandomUser API**, the leading generator for realistic user profiles. By connecting RandomUser.me to your agent, you transform complex dummy data generation into a natural conversation. Your agent can instantly generate thousands of user records, audit location patterns, and retrieve profile pictures without you ever touching a technical script. Whether you are building realistic prototypes or testing application scalability, your agent acts as a real-time data architect, ensuring your test environments are always powered by diverse, high-quality records.

### What you can do

- **Persona Auditing** — Generate comprehensive user profiles, including names, emails, and phone numbers, to maintain a clear view of demographic diversity.
- **Location Oversight** — Retrieve detailed geographic metadata for random users, including street addresses and city coordinates.
- **Seeded Discovery** — Use specific seeds to generate the same set of users consistently across different test cycles.
- **Linguistic Discovery** — List all supported nationalities in the RandomUser catalog to identify regional persona markers.
- **Visual Intelligence** — Retrieve direct links to high-quality profile pictures for any generated user record.

### How it works

1. Subscribe to this server
2. No API Key required (RandomUser is a free and open service)
3. Start managing your persona intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Engineers** — monitor test data quality and retrieve realistic user metadata straight from your workflow.
- **Designers** — verify UI layouts with diverse names and profile pictures without manual searching.
- **Product Managers** — perform rapid audits of prototype personas and identify demographic gaps through natural language.
- **Operations Leads** — automate persona data querying to orchestrate cross-functional development teams smoothly.


## Available Tools
- **check_api_status**: Check if the RandomUser API is operational
- **get_random_users**: Generate random user profiles with names, emails, and locations
- **get_seeded_users**: Generate the same random users using a specific seed string
- **list_supported_nationalities**: List all country codes supported by RandomUser API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RandomUser API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate 5 random female users from 'UK' using RandomUser API."

**🤖 AI Agent:**
> I've generated 5 female personas from the UK! They include names like 'Emma Smith' and 'Sarah Jones', complete with British addresses and profile pictures. Would you like the full JSON details?

---

**👤 You:**
> "Generate a random user with seed 'vinkius_test'."

**🤖 AI Agent:**
> I've retrieved the user for seed 'vinkius_test'. This will return the same persona every time you use this seed. Notable details include the name and city. Would you like me to check another seed?

---

**👤 You:**
> "List all nationalities supported by RandomUser."

**🤖 AI Agent:**
> I've scanned the nationality catalog. It includes 17 countries, from Australia (AU) and Brazil (BR) to the United States (US). I can help you generate users for any of these specific regions.


## Installation & Usage

To install and use the **RandomUser API** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/randomuser-api](https://vinkius.com/mcp/randomuser-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
