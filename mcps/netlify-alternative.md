# Netlify MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/netlify-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/netlify-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/netlify-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Modern web development platform — manage sites, deploys, and forms via AI.

## Description
Empower your AI agent to orchestrate your entire web infrastructure with **Netlify**. This unified server provides your agent with instant access to site management, deployment tracking, and serverless form processing. Your agent can instantly list your active sites, audit deployment technicalities, and trigger new builds without you ever touching the Netlify UI. Whether you are monitoring build pipelines or managing environment variables across multiple projects, your agent acts as a dedicated DevOps engineer through natural conversation.

### What you can do

- **Site Management** — List all sites in your account and retrieve detailed metadata, including production URLs.
- **Deployment Auditing** — Fetch complete deployment history and technical details for any site or specific build.
- **Automation & Builds** — Trigger new production builds using pre-configured build hooks and monitor their status.
- **Form Processing** — Retrieve lists of active forms and audit recent submissions from your users in real-time.
- **Secrets & Config** — List environment variables for your accounts and sites to verify configuration drift.

### How it works

1. Subscribe to this server
2. Enter your Netlify Personal Access Token
3. Start managing your web infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web Developers & Teams** — instantly retrieve site statuses and audit deploys during the development cycle.
- **DevOps Engineers** — automate infrastructure checks and monitor build pipelines through natural language.
- **Project Managers** — track the progress of site updates and review form submissions without technical logins.
- **SaaS Operators** — integrate Netlify workflows into internal tools via an AI-guided interface.
- **Marketing Teams** — monitor lead generation forms and site availability for global campaigns.


## Available Tools
- **get_deploy_details**: Get deploy details
- **get_site_details**: Get site details
- **list_deploys**: List site deploys
- **list_env_vars**: List environment variables
- **list_forms**: List site forms
- **list_build_hooks**: List build hooks
- **list_sites**: List all Netlify sites
- **list_form_submissions**: List form submissions
- **trigger_site_build**: Trigger a site build


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Netlify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all sites in my Netlify account."

**🤖 AI Agent:**
> Retrieving your site directory... You currently have 5 active sites, including 'marketing-landing' and 'docs-portal'. Would you like to check the latest deploy status for any of them?

---

**👤 You:**
> "Show the last 5 deploys for site 'marketing-landing'."

**🤖 AI Agent:**
> Fetching deploy history... The most recent deploy was successful 2 hours ago. I see 4 other production builds from yesterday. I can provide the specific deploy IDs if you need to audit them.

---

**👤 You:**
> "Trigger a new build for site 'docs-portal' using the 'production' hook."

**🤖 AI Agent:**
> Initiating build for 'docs-portal'... The build request has been accepted by Netlify. I'll monitor the status for you. It should be live in a few minutes.


## Installation & Usage

To install and use the **Netlify** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/netlify-alternative](https://vinkius.com/mcp/netlify-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
