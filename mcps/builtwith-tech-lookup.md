# BuiltWith Tech Lookup MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/builtwith-tech-lookup)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/builtwith-tech-lookup-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/builtwith-tech-lookup-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Universal website technology intelligence — detect CMS, analytics, and frameworks via AI.

## Description
Equip your AI agent with the industry standard for website technology profiling through the **BuiltWith** MCP server. This integration provides instant access to the technology stack of millions of domains. Your agent can identify the Content Management System (CMS), analytics tools, advertising networks, hosting providers, and JavaScript frameworks used by any website. Whether you are conducting lead qualification, competitive research, or auditing digital infrastructure, your agent acts as a dedicated technical architect through natural conversation.

### What you can do

- **Tech Stack Profiling** — Retrieve a comprehensive list of all technologies used by a specific domain.
- **CMS Detection** — Identify if a site is running on WordPress, Shopify, Magento, or other platforms.
- **Analytics Auditing** — Discover which tracking and data tools are integrated into a website.
- **Infrastructure Discovery** — Identify hosting, CDN, and security providers for any digital property.

### How it works

1. Subscribe to this server
2. Enter your BuiltWith API Key (get it at builtwith.com)
3. Start profiling websites from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **B2B Sales Teams** — qualify leads based on the technologies they already use.
- **Web Developers & Agency Owners** — research competitor stacks and identify migration opportunities.
- **Security Researchers** — identify the infrastructure and third-party services of target domains.
- **Market Analysts** — track the adoption trends of specific SaaS and web technologies.


## Available Tools
- **get_domain_company_info**: Uses the Company API.

Get company information for a domain
- **get_free_domain_profile**: Does not consume premium credits.

Get basic technology categories for a domain
- **get_domain_keywords**: Uses the Keywords API.

Get keyword profile for a domain
- **get_tech_domain_lists**: Uses the Lists API.

Get lists of domains using a specific technology
- **get_domain_relationships**: Uses the rv2 Relationships API.

Get infrastructure relationships for a domain
- **get_tech_trends**: g., Shopify, React). Uses the v6 Trends API.

Get usage trends for a technology
- **get_domain_trust**: Uses the Trust API.

Get trust indicators for a domain
- **lookup_domain_tech**: Uses the v22 Domain API.

Lookup complete technology stack for a domain


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BuiltWith Tech Lookup** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Lookup the tech stack for 'airbnb.com'."

**🤖 AI Agent:**
> Retrieving technology profile for Airbnb... I've found that they use several key technologies including React, various Google Analytics trackers, and Akamai for CDN. Would you like to see the full list of advertising networks?

---

**👤 You:**
> "Identify the CMS used by 'techcrunch.com'."

**🤖 AI Agent:**
> Checking TechCrunch... This site is powered by WordPress VIP. It also utilizes various VIP-specific plugins and high-performance hosting infrastructure.

---

**👤 You:**
> "Does 'tesla.com' use any marketing automation tools?"

**🤖 AI Agent:**
> I've analyzed the Tesla domain. They are using several marketing and data tools, including Google Tag Manager and custom internal systems. I don't see any standard third-party marketing automation platforms like Marketo or Pardot currently active.


## Installation & Usage

To install and use the **BuiltWith Tech Lookup** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/builtwith-tech-lookup](https://vinkius.com/mcp/builtwith-tech-lookup)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
