# Infracost MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/infracost)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Cloud cost estimates for Terraform — manage cost guardrails, tagging policies, and custom enterprise price books directly through your AI agent.

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


## Available Tools (13)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Infracost** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all cost guardrails for the organization 'acme-corp'."

**🤖 AI Agent:**
> I've retrieved the guardrails for 'acme-corp'. You have two active rules: 1. A $500 increase threshold that blocks PRs, and 2. A $5,000 total monthly budget alert.

---

**👤 You:**
> "Create a new guardrail for 'acme-corp' that triggers when cost increase exceeds $200 and blocks the PR."

**🤖 AI Agent:**
> Successfully created the guardrail. Any Pull Request in 'acme-corp' that increases monthly costs by more than $200 will now be automatically blocked until approved.

---

**👤 You:**
> "Update the tagging policy for 'acme-corp' to make the 'Environment' tag mandatory."

**🤖 AI Agent:**
> I've updated the tagging policy for 'acme-corp'. The 'Environment' tag is now marked as mandatory for all resources managed under this policy.


## ❓ FAQ

**Q: How can I see all active cost guardrails for my organization?**
You can use the `list_guardrails` tool by providing your organization slug. The agent will return a list of all configured thresholds, including cost increase limits and whether they block PRs.

**Q: Can I enforce mandatory tags for my cloud resources using this server?**
Yes! Use the `update_tagging_policy` tool to define mandatory tag keys and allowed values. This helps maintain standards across all your repositories.

**Q: Is it possible to block expensive Pull Requests automatically?**
Absolutely. When using `create_guardrail` or `update_guardrail`, you can set the `blockPr` parameter to true. This ensures that any infrastructure change exceeding your budget cannot be merged without review.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/infracost](https://vinkius.com/mcp/infracost)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Infracost** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `infracost` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Infracost** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "infracost": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
