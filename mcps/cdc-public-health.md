# CDC Public Health / 美国疾控中心 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cdc-public-health)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cdc-public-health-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cdc-public-health-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

U.S. CDC official health resources — search media, audit topics, and get health recommendations via AI.

## Description
Empower your AI agent to orchestrate your public health research and content syndication with the **U.S. Centers for Disease Control and Prevention** (CDC). By connecting the CDC to your agent, you transform complex health resource searching, topic auditing, and evidence-based recommendation retrieval into a natural conversation. Your agent can instantly retrieve detailed media metadata, access comprehensive health topic lists, and even provide personalized health recommendations from the official MyHealthfinder API without you ever needing to navigate multiple government portals. Whether you are conducting academic research or coordinating a public health awareness campaign, your agent acts as a real-time health data coordinator, providing accurate results from a single, authorized source.

### What you can do

- **Media Orchestration** — Search the vast CDC library for articles, infographics, and HTML resources.
- **Content Syndication** — Retrieve HTML embed codes to share official health content directly on your platforms.
- **Topic Auditing** — Access the complete catalog of health topics and their associated metadata.
- **Health Recommendations** — Retrieve personalized, evidence-based health tips using age and gender parameters.
- **Multilingual Support** — Access resources in various languages supported by the CDC Content Services.

### How it works

1. Subscribe to this server
2. Optionally enter your HHS API Key for enhanced access
3. Start managing your health data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Health Researchers & Educators** — automate the gathering of official health metadata and resources through natural language.
- **Content Managers** — coordinate the syndication of official health content directly from your workspace.
- **Developers** — integrate professional-grade public health APIs into your AI-driven daily routines.
- **Public Health Advocates** — stay updated with the latest published resources and recommendations.


## Available Tools
- **get_media_details**: Get media item info
- **get_recent_health_media**: Get latest media items
- **get_syndication_html**: Get embed code for media
- **get_topic_metadata**: Get topic details
- **list_health_topics**: List public health topics
- **list_supported_languages**: List available languages
- **search_health_media**: ) by keyword.

Search CDC media items
- **search_hhs_resources**: Search HHS Digital Media


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CDC Public Health / 美国疾控中心** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for CDC resources about 'Influenza' and show me the latest articles."

**🤖 AI Agent:**
> I've searched the CDC library for 'Influenza'. I found several resources, including the 'Key Facts About Seasonal Flu' article (ID: `88210`) and a recent infographic. Would you like the detailed metadata or the HTML embed code for one of these?

---

**👤 You:**
> "Get health recommendations for a 35-year-old female."

**🤖 AI Agent:**
> Based on official health guidelines for a 35-year-old female, recommended preventative measures include regular blood pressure screenings, cervical cancer screenings, and staying updated with seasonal vaccines. Would you like more details on any of these topics?

---

**👤 You:**
> "List the most recently published health resources from the CDC."

**🤖 AI Agent:**
> I've retrieved the latest health resources. Recent publications include updates on 'Travel Health Notices', 'Emerging Infections Reports', and new dietary guidelines for parents. Would you like to see the description for the travel notices?


## Installation & Usage

To install and use the **CDC Public Health / 美国疾控中心** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cdc-public-health](https://vinkius.com/mcp/cdc-public-health)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
