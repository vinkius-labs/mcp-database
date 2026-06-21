# Agify MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/agify)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/agify-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/agify-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Predict the age of a person based on their first name using the Agify.io API.

## Description
Connect your AI agent to **Agify.io** to instantly estimate the age of individuals or groups based on their first names. This server provides powerful demographic intelligence for data enrichment and user profiling.

### What you can do

- **Individual Prediction** — Estimate the age of a single person by providing their first name.
- **Country Scoping** — Improve accuracy by narrowing the prediction to a specific country using ISO codes.
- **Batch Processing** — Predict ages for up to 10 names in a single request for efficient data analysis.
- **Probability Metrics** — Receive not just an age, but the data count used to generate the prediction.

### How it works

1. Subscribe to this server
2. Enter your Agify API Key (optional for limited testing)
3. Start predicting demographics from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — Enrich user databases with estimated demographic information.
- **Marketing Teams** — Segment leads and audiences based on name-derived age estimates.
- **Developers** — Build smarter onboarding flows or personalization engines without asking for birth dates.


## Available Tools
- **predict_age_batch**: Predict the ages of multiple people based on their first names
- **predict_age**: Optionally scope by country.

Predict the age of a person based on their first name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Predict the age for the name 'Michael'."

**🤖 AI Agent:**
> Based on the Agify database, the estimated age for 'Michael' is 44 years old (based on 233,482 data points).

---

**👤 You:**
> "What is the estimated age for 'Isabella' in Italy (IT)?"

**🤖 AI Agent:**
> In Italy, the name 'Isabella' has an estimated age of 52 years.

---

**👤 You:**
> "Predict the ages for these names: 'John', 'Emma', and 'Liam'."

**🤖 AI Agent:**
> I've processed the batch: 'John' is estimated at 51, 'Emma' at 34, and 'Liam' at 21.


## Installation & Usage

To install and use the **Agify** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/agify](https://vinkius.com/mcp/agify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
