# Redox MCP Server

Connect to the Redox healthcare API to search patients, retrieve clinical conditions, and write back observations directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/redox)

## Overview
**Category:** developer-tools
**Tools Count:** 4

## Description
Integrate your **Redox** environment with any AI agent to streamline healthcare interoperability. This server allows you to interact with clinical data using both FHIR standards and Redox Data Models through natural language.

### What you can do

- **Patient Discovery** — Search for patient records across connected healthcare systems using specific identifiers and destination slugs.
- **Clinical Insights** — Retrieve active diagnoses and conditions (problem lists) for specific patients to provide medical context.
- **Clinical Writeback** — Save vitals and clinical observations back to the EHR by sending structured FHIR bundles.
- **Data Model Events** — Send asynchronous notifications or synchronous queries using standardized Redox JSON Data Models for broad interoperability.
- **Environment Management** — Seamlessly switch between development and production environments for testing and deployment.

### How it works

1. Subscribe to this server
2. Enter your Redox API Key
3. Start querying patient data or posting clinical observations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **HealthTech Developers** — Test clinical integrations and verify FHIR resource mapping directly from your coding environment.
- **Clinical Operations** — Quickly look up patient conditions or identifiers without navigating complex EHR interfaces.
- **Digital Health Startups** — Accelerate the development of AI-driven medical assistants by providing them with real-time access to clinical data.


## Available Tools
- **create_observation**: Save vitals or observations (Writeback)
- **post_data_model**: Send a Redox Data Model API event
- **search_condition**: g., problem-list-item) associated with a specific patient ID.

Retrieve diagnoses/conditions for a patient
- **search_patient**: Search for a patient in Redox FHIR API


## Installation & Usage

To install and use the **Redox** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/redox](https://vinkius.com/mcp/redox)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
