# Codefresh MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/codefresh)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ship-it](../categories/ship-it.md)

Manage CI/CD and GitOps via Codefresh — track pipelines, trigger builds, and monitor delivery clusters directly from any AI agent.

## Description
Connect your **Codefresh** account to any AI agent and take full control of your CI/CD and cloud-native delivery through natural conversation. Streamline how you automate and monitor software deployments natively.

### What you can do

- **Pipeline Oversight** — List and retrieve details for all CI/CD pipelines including their configurations natively
- **Build Management** — Trigger new builds for specific pipelines and specify branches or variables flawlessly
- **Workflow Intelligence** — Access detailed status and execution info for recent builds (workflows) flawlessly
- **Cluster Logistics** — Monitor all connected Kubernetes and delivery clusters to verify deployment targets securely
- **Environment Auditing** — List shared contexts, including secrets and variables, used in your workflows securely
- **integrated Visibility** — Retrieve detailed build metadata and user profile information directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Codefresh API Key (found in User Settings > API Keys)
3. Start managing your CI/CD pipelines from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps Engineers** — monitor pipeline health and trigger manual builds using natural language
- **Release Managers** — audit deployment success rates and cluster status without opening the dashboard
- **Software Developers** — quickly look up build execution details and verify environmental contexts straight from their chat interface
- **Infrastructure Teams** — verify Kubernetes cluster connectivity and monitor GitOps delivery


## Available Tools
- **get_build_execution_details**: Get detailed status and execution info for a specific build
- **get_my_codefresh_profile**: Retrieve information about the authenticated user and account
- **get_pipeline_configuration**: Get detailed information for a specific pipeline
- **list_codefresh_builds**: List all recent builds (workflows) in the account
- **list_delivery_clusters**: List all connected Kubernetes/Delivery clusters
- **list_shared_contexts**: List all shared environment contexts (secrets, variables)
- **list_codefresh_pipelines**: List all CI/CD pipelines in the account
- **trigger_codefresh_build**: Trigger a new build for a specific pipeline


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Codefresh** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Codefresh pipelines."

**🤖 AI Agent:**
> Retrieving your pipelines... I found 5 active pipelines: 'main-app-deploy', 'api-service-ci', 'frontend-build', and 2 others. Which one would you like to run?

---

**👤 You:**
> "Trigger the 'api-service-ci' pipeline on the 'develop' branch."

**🤖 AI Agent:**
> Triggering build for api-service-ci (branch: develop)... The build has been successfully started in Codefresh. The build ID is '605c...123'. I can monitor the progress for you.

---

**👤 You:**
> "Show me the status of my recent builds."

**🤖 AI Agent:**
> Checking recent builds... I found 5 items. 4 were successful and 1 for 'frontend-build' failed with a 'STAGED_EXPIRED' status. Would you like to see the logs for the failed build?


## ❓ FAQ

**Q: Can I trigger a pipeline run for a specific branch?**
Yes! Use the `trigger_codefresh_build` tool. You can provide the pipeline ID and specify the branch name in the payload. The agent will instruct Codefresh to start the build immediately.

**Q: How do I see the status of all my Kubernetes clusters in Codefresh?**
Use the `list_delivery_clusters` tool. Your agent will fetch all connected clusters, showing you which targets are available for deployment and their current health status.

**Q: Where do I find my Codefresh API Key?**
Log in to Codefresh, click on your profile icon, go to **User Settings**, and select **API Keys**. You can generate and copy a new token from that section.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/codefresh](https://vinkius.com/mcp/codefresh)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Codefresh** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `codefresh` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Codefresh** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "codefresh": {
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
