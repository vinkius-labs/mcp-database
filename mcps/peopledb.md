# PeopleDB MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/peopledb)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/peopledb-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/peopledb-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Supercharge your lead generation by letting AI agents enrich B2B profiles and verify contact data instantly.

## Description
Empower your sales and data teams by integrating People Data Labs directly into your AI workflows. Your AI agent can tap into a database of over 3 billion records to automatically enrich incomplete lead profiles, verify email deliverability on the fly, and standardize messy CRM records before outreach campaigns.

### What you can do
- Enrich person and company profiles
- Search people and companies with SQL-like filters
- Verify email deliverability
- Identify people from partial data
- Clean and standardize names, locations, and company names

### How it works
1. Subscribe to PeopleDB (PeopleDataLabs)
2. Generate your API key in the dashboard
3. Start enriching your contacts securely via Vinkius

### Who is it for?
Ideal for sales teams, marketers, and developers looking to clean and enrich B2B contact lists instantly.


## Available Tools
- **autocomplete**: Autocomplete field values
- **bulk_enrich_people**: Bulk enrich people
- **clean_company**: Clean a company name
- **clean_location**: Clean a location
- **clean_name**: Clean a name
- **enrich_company**: Enrich a company
- **enrich_person**: Enrich a person
- **get_balance**: Check credit balance
- **identify_person**: Identify a person
- **search_companies**: Search companies
- **search_people**: Search people
- **verify_email**: Verify an email


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PeopleDB** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Enrich the person with email john@company.com on PeopleDB"

**🤖 AI Agent:**
> I've enriched the profile for john@company.com. His name is John Doe, and he currently works as a Senior Software Engineer at TechCorp. Would you like to see his LinkedIn profile and full skill set?

---

**👤 You:**
> "Is the email contact@example.com valid and deliverable?"

**🤖 AI Agent:**
> Yes, the email contact@example.com is valid and highly deliverable. It is tied to an active MX record and does not appear to be a catch-all.

---

**👤 You:**
> "Find all CTOs in SaaS companies based in San Francisco"

**🤖 AI Agent:**
> I found 2,150 CTOs in SaaS companies based in San Francisco. Do you want me to filter them further by company size or specific skills like 'Machine Learning'?


## Installation & Usage

To install and use the **PeopleDB** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/peopledb](https://vinkius.com/mcp/peopledb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
