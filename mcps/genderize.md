# Genderize MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/genderize)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/genderize-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/genderize-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Predict the gender of a person based on their first name via AI agents with Genderize.io.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Genderize** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Estimate the gender for the name 'Peter'."

**🤖 AI Agent:**
> Predicting gender... For the name 'Peter', Genderize.io estimates a 'male' identity with 99% probability based on 165,452 records.

---

**👤 You:**
> "Predict the genders for these names: ['Alice', 'Bob', 'Charlie']."

**🤖 AI Agent:**
> Processing names... I've retrieved estimations for all 3 names: Alice (female, 98%), Bob (male, 99%), and Charlie (male, 56%).

---

**👤 You:**
> "What is the predicted gender for 'Sasha' in Russia (RU)?"

**🤖 AI Agent:**
> Checking local patterns... In Russia (RU), the name 'Sasha' is estimated as 'male' with 64% probability.


## Installation & Usage

To install and use the **Genderize** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/genderize](https://vinkius.com/mcp/genderize)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
