# Vercel MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vercel)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Bring your Vercel deployment infrastructure into chat. Control project domains, trigger manual builds, and inspect deployment status natively.

## Description
Embed your **Vercel** continuous integration ecosystem into the mind of your AI agent. Perform advanced DevOps commands via chat, bypassing the Vercel web UI and checking application states natively within your IDE.

### What you can do

- **Project Control** — Command your assistant to list your current architecture portfolio, examine Git environment settings, or spin up new Vercel boundary projects dynamically from the chat window.
- **Deployment Management** — Trace live builds. Request the active CI/CD execution status on recent commits, fetch preview URLs upon build completion, or ruthlessly cancel stalled serverless compilations.
- **Manual Deploy Triggers** — Skip the Github pushes. You can explicitly command a forced build on specific repository tags directly through the MCP integration when hot-fixing.
- **Domain Auditing** — Ask the agent to map out the DNS and SSL status of your custom root domains, parsing current subdomain routing alias tables clearly.

### How it works

1. Subscribe your workspace to this connector
2. Introduce your personal Vercel API Token for authorization
3. Engage Claude or Cursor to manage deployment lifecycles seamlessly

### Who is this for?

- **Frontend Engineers** — trigger new manual Next.js deployments inside Cursor directly after fixing a tricky CSS bug, tracking the CI steps silently while coding the next feature.
- **DevOps Architects** — perform rapid audits of linked domain structures and DNS alias health checks across the organization's array using basic conversational inputs.
- **Quality Assurance** — instantly pull the most recent Preview URL generated from the target branch staging deployments without hunting for the Vercel notification link.


## Available Tools (10)
- **cancel_active_build**: Aborts an ongoing Vercel compilation pipeline
- **trigger_github_deployment**: Provide the project name and Git ref.

Triggers a new Vercel build from a specific GitHub reference
- **create_project**: Provide a name and framework slug.

Creates a new Vercel project
- **list_account_domains**: Lists high-level apex domains managed by Vercel
- **list_projects**: Lists all Vercel projects in the account
- **delete_project**: This action is irreversible.

Permanently removes a Vercel project
- **get_deployment_details**: Retrieves details for a specific deployment execution
- **get_project_details**: Retrieves detailed configuration for a specific project
- **list_project_aliases**: Lists specific subdomain routing mappings for a project
- **list_deployments**: Lists recent CI/CD builds for a specific project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vercel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all root domains connected to my Vercel infrastructure."

**🤖 AI Agent:**
> I've queried the apex domains across your environment. You have 3 custom domains actively bound: `production-agent.com`, `internal-tools.io`, and `legacy-blog-marketing.net`. All three signify successful certificate validations.

---

**👤 You:**
> "Create a manual deploy on the 'billing-service' project pulling directly from the 'main' branch on GitHub repo '341xyz'."

**🤖 AI Agent:**
> I've successfully triggered a queued manual compilation for 'billing-service' using your target GitHub parameters. 

Vercel has acknowledged the deployment intent. The new processing ID assigned to this task is `dpl_H3vM4Q...`. You can poll `get_deployment_details` intermittently with this string or I can check again for you in 3 minutes if you'd prefer.

---

**👤 You:**
> "Check the status of deployment 'dpl_827a' and give me its exact live preview URL if ready."

**🤖 AI Agent:**
> I've checked deployment `dpl_827a`. Good news – Vercel marks its `readyState` as fully `READY`. There were zero pipeline errors.

You can access your newly compiled live preview here: [https://billing-service-pr-12-test.vercel.app](https://billing-service-pr-12-test.vercel.app)


## ❓ FAQ

**Q: Can I cancel a stuck Vercel deployment directly from my chat window?**
Yes. If a build hangs, simply find its ID via `list_deployments` and tell the agent: `Abort the deployment execution 'dpl_9B...'`. The `cancelDeploymentTool` intercepts and kills the remote CI task instantly.

**Q: How do I get the Preview URL of a newly built branch?**
Instruct the AI manually: `Grab the deployment details for 'dpl_xx3'`. Using the `getDeploymentTool`, the agent will output the associated generated live `url` property for you to click without going to the dashboard notifications.

**Q: Can I spin up an empty Vercel project programmatically through the agent before I even connect my repository?**
Yes. Run the prompt: `Create a new Next.js project on Vercel named 'test-saas'`. The agent initiates `createProjectTool`, and Vercel will instantly return its new unique Project GUID, ready to be linked to code whenever you wish.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vercel](https://vinkius.com/mcp/vercel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vercel** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vercel` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vercel** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vercel": {
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
