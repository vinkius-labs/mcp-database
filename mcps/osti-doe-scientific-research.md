# OSTI (DOE Scientific Research) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/osti-doe-scientific-research)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/osti-doe-scientific-research-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/osti-doe-scientific-research-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access Department of Energy research, datasets, and scientific publications. Search records, retrieve metadata, and manage DOI registrations.

## Description
Connect to the **Office of Scientific and Technical Information (OSTI)** to query the US Department of Energy's vast research output. This MCP server allows AI agents to navigate millions of research records and datasets through natural conversation.

### What you can do

- **Research Search** — Query OSTI.GOV for publications, reports, and conference papers using authors, titles, or specific identifiers.
- **Dataset Discovery** — Search the DOE Data Explorer specifically for scientific datasets and retrieve detailed metadata for data-driven insights.
- **Record Inspection** — Fetch comprehensive bibliographic data and full-text availability for specific records using unique OSTI IDs.
- **DOI Management** — Reserve and submit Digital Object Identifiers (DOIs) via the E-Link API for DOE-funded scientific research and data.
- **Advanced Filtering** — Narrow down results by sponsoring organization, research organization, or specific publication date ranges.

### How it works

1. Subscribe to this server
2. (Optional) Enter your OSTI E-Link Token for DOI reservation and submission features
3. Start searching and analyzing scientific data directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Researchers & Academics** — quickly find relevant DOE-funded literature and datasets without manual portal searching
- **Data Scientists** — discover and inspect metadata for scientific datasets to fuel analysis and modeling
- **Grant Administrators** — manage DOI registrations and verify record submissions for funded projects


## Available Tools
- **get_data_explorer_record**: Get a single DOE Data Explorer record by ID
- **get_osti_record**: Get a single OSTI.GOV record by ID
- **reserve_doi**: Requires minimal metadata.

Reserve a DOI via E-Link API
- **search_data_explorer_records**: Search DOE Data Explorer records (datasets)
- **search_osti_records**: Search OSTI.GOV records
- **submit_record**: Submit/Update a record and register DOI via E-Link API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OSTI (DOE Scientific Research)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for research papers about 'quantum computing' published in 2023."

**🤖 AI Agent:**
> I've found several records for 'quantum computing' from 2023. Notable entries include 'Quantum Error Correction in Scalable Architectures' (OSTI ID: 1982341) and 'Advances in Superconducting Qubits'. Would you like the full details for any of these?

---

**👤 You:**
> "Find scientific datasets related to 'solar irradiance' in the DOE Data Explorer."

**🤖 AI Agent:**
> Searching the Data Explorer... I've identified 3 datasets. The most relevant is 'High-Resolution Solar Irradiance Data for the Southwestern US' (OSTI ID: 150432). It includes hourly measurements from 2018-2022.

---

**👤 You:**
> "Get the complete metadata for OSTI record ID 1015678."

**🤖 AI Agent:**
> Retrieving record 1015678... This is a technical report titled 'Atmospheric Radiation Measurement (ARM) User Facility'. It was authored by the Pacific Northwest National Laboratory and sponsored by the Office of Science.


## Installation & Usage

To install and use the **OSTI (DOE Scientific Research)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/osti-doe-scientific-research](https://vinkius.com/mcp/osti-doe-scientific-research)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
