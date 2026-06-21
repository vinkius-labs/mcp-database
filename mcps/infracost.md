# Infracost MCP Server

Cloud cost estimates for Terraform — manage cost guardrails, tagging policies, and custom enterprise price books directly through your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/infracost)

## Overview
**Category:** loved-by-devs
**Tools Count:** 13

## Description
Connect **Infracost** to your AI agent to bring financial visibility and governance to your Infrastructure as Code (IaC) workflows. Prevent cloud cost surprises before they happen.

### What you can do

- **Cost Guardrails** — List, create, and manage guardrails that trigger alerts or block Pull Requests when cost increases exceed your defined thresholds.
- **Tagging Governance** — Enforce organizational standards by updating tagging policies, ensuring all cloud resources are correctly attributed to departments or projects.
- **Custom Pricing** — Manage enterprise-specific price books for AWS and Azure to ensure cost estimates reflect your actual negotiated discounts.
- **Business Context** — Upload custom properties from external systems like ServiceNow or Backstage to map cloud costs to your internal organizational hierarchy.
- **Pricing Queries** — Programmatically query cloud pricing data to compare costs across different resource types and regions.

### How it works

1. Subscribe to this server
2. Enter your Infracost API Token
3. Start managing your cloud governance from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — automate the enforcement of cost policies and tagging standards directly within the CI/CD flow.
- **FinOps Teams** — gain real-time visibility into infrastructure spend and manage custom enterprise discounts without manual spreadsheets.
- **Engineering Managers** — set budget thresholds and receive automated summaries of cost impacts for proposed infrastructure changes.


## Available Tools
- **list_guardrails**: List all guardrails for an organization
- **query_pricing**: Provide a valid GraphQL query string.

Query the Cloud Pricing API using GraphQL
- **create_guardrail**: Create a new guardrail
- **create_price_book**: Create a custom price book for an enterprise
- **delete_guardrail**: Delete a guardrail
- **get_guardrail**: Get a specific guardrail by ID
- **get_price_book_files_url**: Use the returned URL to PUT the CSV file.

Get a presigned URL to upload a price book CSV
- **get_price_book**: Poll this to wait for SUCCESS status.

Get the status and details of a price book
- **ingest_price_book**: Call this after uploading the CSV to the presigned URL.

Trigger ingestion of an uploaded price book CSV
- **update_guardrail**: Update an existing guardrail
- **update_organization**: Pass the customPriceBookId to activate it.

Update organization settings, such as activating a custom price book
- **update_tagging_policy**: Update allowed tag values for a tagging policy
- **upload_custom_properties**: g., from ServiceNow or Backstage) for cost attribution. Provide raw CSV data.

Upload custom business properties via CSV


## Installation & Usage

To install and use the **Infracost** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/infracost](https://vinkius.com/mcp/infracost)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
