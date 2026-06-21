# RxNorm Drug Terminology MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rxnorm-drug-terminology)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/rxnorm-drug-terminology-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/rxnorm-drug-terminology-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Universal drug nomenclature intelligence — resolve clinical drug names and codes via AI.

## Description
Equip your AI agent with the industry-standard terminology for clinical drugs through the **RxNorm** MCP server. This integration provides instant access to the Unified Medical Language System (UMLS) and the National Library of Medicine (NLM) databases. Your agent can normalize drug names, retrieve unique RxCUI identifiers, and explore related drug concepts (ingredients, brands, dose forms). Whether you are auditing electronic health records, normalizing medication lists, or researching clinical drug relationships, your agent acts as a dedicated medical terminologist through natural conversation.

### What you can do

- **Name Normalization** — Resolve ambiguous clinical drug names into standardized RxNorm terminology.
- **Identifier Retrieval** — Fetch unique RxCUI codes for any drug concept in the database.
- **Relationship Mapping** — Explore links between active ingredients, brand names, and clinical doses.
- **Term Auditing** — Summarize and classify medical drug concepts for systematic analysis.

### How it works

1. Subscribe to this server
2. No API Key required (Public Access)
3. Start normalizing drug terms from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Healthcare Software Developers** — normalize drug names in medical applications and databases.
- **Clinical Data Scientists** — ensure data integrity by mapping drug concepts to standardized codes.
- **Medical Librarians & Researchers** — navigate the complex web of pharmaceutical nomenclature.
- **Health Tech Auditors** — verify the accuracy of medication records against official terminologies.


## Available Tools
- **get_drug_properties**: Get all properties for an RxCUI
- **get_rxcui_by_name**: Get RxCUI for a drug name
- **get_drug_spelling_suggestions**: Get spelling suggestions for a drug name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RxNorm Drug Terminology** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Normalize the drug name 'Tylenol'."

**🤖 AI Agent:**
> Searching RxNorm... I've resolved 'Tylenol' to several standardized concepts. The primary clinical concept is Acetaminophen (RxCUI: 161). Would you like to see the different dose forms and strengths available?

---

**👤 You:**
> "What is the RxCUI for 'Amoxicillin 500mg capsule'?"

**🤖 AI Agent:**
> Retrieving normalized ID... The specific RxCUI for Amoxicillin 500 MG Oral Capsule is 308182. This identifier can be used for consistent record keeping and clinical data mapping.

---

**👤 You:**
> "Show related drug concepts for 'Lipitor'."

**🤖 AI Agent:**
> Inspecting related terms... 'Lipitor' is a brand name for the ingredient Atorvastatin (RxCUI: 83367). It is available in various clinical drug components and packs. Would you like a list of all strengths and forms linked to this brand?


## Installation & Usage

To install and use the **RxNorm Drug Terminology** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rxnorm-drug-terminology](https://vinkius.com/mcp/rxnorm-drug-terminology)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
