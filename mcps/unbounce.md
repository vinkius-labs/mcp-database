# Unbounce MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/unbounce)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Automate marketing tasks via Unbounce — retrieve landing pages, fetch captured leads, audit performance stats, and manage test variants easily.

## Description
Connect your **Unbounce** marketing workflows to any AI agent and take full enterprise control over global landing pages, captured leads routing, and real-time conversion monitoring natively via conversational commands.

### What you can do

- **Project & Sub-Account Control** — Interrogate your organization's hierarchy grouping, natively verifying assigned domains before pushing any pages live
- **Real-Time Lead Extraction** — Fetch form submission pipelines continuously directly from targeted pages without battling CSV exports
- **Variant Auditing** — Read A/B testing splits mapped across single pages to identify statistically significant conversions rapidly
- **Lead Obliteration** — Trigger raw data-privacy deletions directly across specific captured accounts dropping rogue leads off the servers 

### How it works

1. Subscribe manually to this core server context
2. Introduce your Personal Developer Unbounce API Auth Token into the connection setup
3. Start mapping live conversion tracking or list pulling natively inside Claude or your specific IDE space

Manage hundreds of lead generation funnels automatically by prompting the LLM instead of suffering visually heavy interface delays.

### Who is this for?

- **Growth Marketers** — query the system directly inside chat windows pulling performance stats isolating top-performing split variations in 5 seconds
- **Sales Development** — fetch new lead details natively triggering follow-ups faster checking EXACT form entries avoiding unformatted messy exports
- **Marketing Agencies** — list hundreds of client specific domains spanning dynamic sub-accounts cleanly auditing deployment checks effortlessly


## Available Tools (4)
- **domains**: List custom domains configured in the account
- **leads**: List leads/submissions for a specific landing page
- **pages**: List landing pages in Unbounce
- **sub_accounts**: List sub-accounts available to the user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Unbounce** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Please list the verified domains available for publication underneath the specific main active sub-account."

**🤖 AI Agent:**
> I've fetched 3 attached domains securely: 'get.vinkius.cloud', 'campaigns.yourstack.com', and a root domain entry for 'product.marketing.io'. Need to list the active pages attached inside any?

---

**👤 You:**
> "Summarize the conversion metrics and variant splits for the 'Enterprise Launch Q3' LP ID."

**🤖 AI Agent:**
> Page Stats fetched! Total audience hits stand at 14,200. Variant A processed a miserable 1.2% conversion rate, but Variant B dominated at 11%, effectively gathering over 1,500 firm leads inherently. Drop Variant A when possible.

---

**👤 You:**
> "Isolate the exact form submission metadata payload for lead ID 7709xxv-1123."

**🤖 AI Agent:**
> Retrieved form values securely for Lead 7709xxv: User email marked 'john.doe@test.com'. Included an arbitrary internal company name input as 'Acme Global'. The request indicates no additional customized checkboxes were marked.


## ❓ FAQ

**Q: Can it retrieve all form submission data (Leads) for a specific landing page in one go?**
Absolutely. Just instruct the agent using the 'list_page_leads' capability, feeding it the specific landing page ID. It directly taps the records returning JSON-wrapped metadata of exactly what your visitors typed in.

**Q: How can I check the performance and stats of a live landing page quickly?**
Simply ask the agent to fetch the page statistics using 'get_page_statistics' with its respective ID. Data elements like bounce rates, overall views vs conversions naturally return into the AI context mapping easy charts.

**Q: Can it query sub-accounts dynamically finding out assigned domains on larger enterprise accounts?**
Yes. First call 'list_sub_accounts' to get raw IDs, then orchestrate 'list_sub_account_domains' recursively across those IDs. In one prompt, your AI audits the entire organizational deployment topology natively.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/unbounce](https://vinkius.com/mcp/unbounce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Unbounce** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `unbounce` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Unbounce** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "unbounce": {
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
