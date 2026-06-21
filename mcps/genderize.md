# Genderize MCP Server

Predict the gender of a person based on their first name via AI agents with Genderize.io.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/genderize)

## Overview
**Category:** developer-tools
**Tools Count:** 8

## Description
Connect your AI agent to the **Genderize.io** database to automate gender estimation through the Model Context Protocol (MCP). Genderize.io is a specialized API that provides statistical probabilities for the gender associated with any first name, backed by a database of over 114 million records. This MCP server enables you to estimate genders for single or multiple names, localized by country, directly through natural conversation.

### Key Features

- **Gender Estimation** — Predict whether a first name is associated with a male or female identity based on global data.
- **Statistical Probability** — Retrieve certainty scores (0.0 to 1.0) and the total data count used for each prediction.
- **Country Localization** — Localize results by providing ISO country codes (e.g., 'US', 'BR', 'GB') to improve accuracy for regional naming patterns.
- **Batch Processing** — Estimate genders for up to 10 names in a single request to process lead lists faster.
- **Regional Helpers** — Quickly check names for specific countries like the USA, Brazil, UK, Spain, and France using dedicated tools.
- **No-Auth Free Tier** — Start using the service immediately with up to 100 free requests per day without an API key.
- **Scale with API Keys** — Optionally provide an API key to access higher rate limits for large-scale data enrichment.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Optional: Enter your Genderize API Key (for higher limits)
3. Start predicting genders from Claude, Cursor, or any MCP client

### Who is this for?

- **Data Analysts & Marketers** — quickly enrich lead lists or CRM data with gender estimations for personalized outreach.
- **Growth Engineers** — automate the localization of user profiles based on naming probabilities via simple AI commands.
- **Developers** — verify naming patterns and statistical distributions without manual API testing.


## Available Tools
- **verify_api_connection**: io API connectivity.

Check connection
- **estimate_gender_brazil**: Predict gender (Brazil)
- **estimate_gender_spain**: Predict gender (Spain)
- **estimate_gender_france**: Predict gender (France)
- **estimate_gender_uk**: Predict gender (UK)
- **estimate_gender**: Predict gender by name
- **estimate_gender_us**: Predict gender (USA)
- **estimate_genders_bulk**: Predict multiple names


## Installation & Usage

To install and use the **Genderize** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/genderize](https://vinkius.com/mcp/genderize)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
