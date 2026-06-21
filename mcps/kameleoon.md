# Kameleoon MCP Server

Manage A/B testing, personalization, and experimentation workflows via AI agents.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/kameleoon)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Empower your AI agents to control your **Kameleoon** experimentation platform. This MCP server enables seamless management of experiments, variations, and audience segments directly from natural language interfaces.

### What you can do

- **Experiment Control** — List all active experiments and drill down into specific configurations and metadata
- **Variation Management** — Inspect A/B variations and their statuses across different digital properties
- **Site Inventory** — Query all sites and properties registered in your account to ensure correct environment targeting
- **Audience Segmentation** — List defined audience segments and targeting rules used for precise traffic allocation
- **Results Triggering** — Request latest results reports to analyze experiment performance on the fly

### How it works

1. Subscribe to this server
2. Enter your Kameleoon Client ID and Client Secret
3. Start managing your A/B tests and personalization from Claude, Cursor, or any MCP client

### Who is this for?

- **Product Managers** — Monitor the status of live experiments and check variants without logging into the Kameleoon dashboard
- **Growth Engineers** — Quickly query targeting rules and custom data dimensions from your IDE
- **Data Analysts** — Automate the retrieval of experiment results and metadata for reporting


## Available Tools
- **create_experiment**: Requires a name and a site ID.

Create a new experiment
- **list_custom_data**: List custom data dimensions
- **list_experiments**: Use this to monitor campaign statuses and identify active experiments.

List all experiments in Kameleoon
- **get_experiment**: Get details for a specific experiment
- **get_site**: Get details for a specific site
- **get_experiment_results**: This is an asynchronous process in the Kameleoon API.

Request a results report for an experiment
- **list_targeting_rules**: List targeting rules
- **list_segments**: List audience segments
- **list_sites**: List all sites in the account
- **list_variations**: ) associated with a specific experiment ID.

List variations for an experiment


## Installation & Usage

To install and use the **Kameleoon** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kameleoon](https://vinkius.com/mcp/kameleoon)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
