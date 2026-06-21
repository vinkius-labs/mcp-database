# Mav MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mav-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mav-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mav-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Let AI text your leads automatically with human-like conversations that schedule appointments and qualify prospects by SMS.

## Description
Connect your **Mav** AI recruiting account to any AI agent and manage candidate screening through natural conversation.

### What you can do

- **Candidate Screening** — Trigger automated AI screening conversations
- **SMS Campaigns** — Launch and manage outbound SMS recruiting campaigns
- **Lead Management** — Browse candidates and their qualification status
- **Engagement Tracking** — Monitor open rates, reply rates, and drop-offs
- **Interview Data** — Access responses and screening transcripts

### How it works

1. Subscribe to this server
2. Enter your Mav API Key
3. Start managing recruiting campaigns from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Recruiters** — automate initial candidate screening at scale
- **Talent Acquisition** — run high-volume SMS outreach campaigns
- **HR Ops** — monitor hiring funnel metrics and candidate engagement


## Available Tools
- **create_lead**: Create a lead and trigger a playbook
- **get_lead**: Get details for a specific lead
- **get_playbook**: Get details for a specific playbook
- **list_activities**: List recent activities/events
- **list_leads**: List all leads
- **list_playbooks**: List all available Mav playbooks
- **opt_out_lead**: Manually opt-out a lead
- **stop_playbook**: Stop a running playbook for a lead
- **update_lead**: Update an existing lead


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mav** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show active SMS campaigns and completion rates."

**🤖 AI Agent:**
> Active Campaigns: 3. 'Retail Store Manager' (450 candidates, 68% reply, 45% completion ⭐). 'Warehouse Staff' (1,200 candidates, 42% reply, 28% completion). 'Customer Support' (300 candidates, 55% reply, 38% completion). Total screened today: 145. Qualified: 42.

---

**👤 You:**
> "Launch a screening campaign for the new Warehouse Staff list."

**🤖 AI Agent:**
> Campaign launched! ✅ Campaign ID: cmp_890. Target list: 'Warehouse_Applicants_Q2' (150 candidates). Screening flow: 'Basic Warehouse Qualification'. First SMS sent to 150 candidates. Estimated completion time: 2-4 hours.

---

**👤 You:**
> "Show screening results and transcripts for qualified candidates."

**🤖 AI Agent:**
> Qualified candidates: 3 (Retail Manager). 1) Sarah J. (Score: 95%, 'Has 5+ years retail management experience. Available immediately.'). 2) Mike T. (Score: 88%, '3 years experience, flexible schedule.'). Transcript for Sarah available: Link to transcript. Move to interview stage?


## Installation & Usage

To install and use the **Mav** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mav-alternative](https://vinkius.com/mcp/mav-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
